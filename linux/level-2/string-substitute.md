# String

There is some data on `Nautilus App Server 3` in `Stratos DC`. Data needs to be altered in several of the files. On `Nautilus App Server 3`, alter the `/home/BSD.txt` file as per details given below:

a. Delete all lines containing word `software` and save results in `/home/BSD_DELETE.txt` file. (Please be aware of case sensitivity)

b. Replace all occurrence of word `the` to `their` and save results in `/home/BSD_REPLACE.txt` file.

`Note:` Let's say you are asked to replace word `to` with `from`. In that case, make sure not to alter any words containing the string itself; for example up**to**, contribu**to**r etc.

1. SSH into App Server 3
   `ssh banner@stapp03`
2. Adjust permission of `/home` directory
   `sudo chmod 777 /home`
3. Replace `software` in BSD.txt > BSD_DELETE.txt
   `grep -v software /home/BSD.txt > /home/BSD_DELETE.txt`
4. Replace `the` to `their` > `BSD_REPLACE.txt`
   `sudo sed 's/\bthe\b/their/g' /home/BSD.txt > /home/BSD_REPLACE.txt`
5. Return permissions of `/home` to original
   `sudo chmod 755 /home`
---
You have successfully completed the challenge.Results have been saved. Ref ID:64072005741b204d59fbe985
August 25, 2023
