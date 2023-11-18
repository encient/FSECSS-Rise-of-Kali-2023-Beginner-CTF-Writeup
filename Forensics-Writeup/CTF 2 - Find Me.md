# Question
Do you know `ls`?

Attachment: `flag.zip`

# Solution
![image](https://github.com/encient/FSECSS-Rise-of-Kali-2023-Beginner-CTF-Writeup/assets/95013757/0f420ee2-8953-426a-94e7-5e5eef54c3a3)

Extract the zip file by using the command `unzip flag.zip`. You will see that there are two files being extracted which is `flag.pdf` and `.password`. However, if you use `ls` to list the files, only `flag.pdf` will be shown. You can use `ls -la` to list the hidden file. Use `cat .password` to get the password of the protected file, and press `Ctrl + A` to select all contents in the file to see the flag (the flag is in white font).

password: `3dkz1V4vvQYxWAn`


# Flag
`ROK{hidd3n_fil3}`
