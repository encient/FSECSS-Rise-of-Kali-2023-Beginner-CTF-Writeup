# Question
Extract the all the files to get the flag.

Attachment: `flag`

# Solution
![image](https://github.com/encient/FSECSS-Rise-of-Kali-2023-Beginner-CTF-Writeup/assets/95013757/64211686-abd0-416d-bdb1-3019efbf3e72)

This challenge is for you to learn how to extract different types of zip files. However, the file does not show what is the file type. Therefore, we have to use `file` command to determine the file type. `file flag` to see the file type and you will know that it is a zip file. Use `unzip flag` to unzip it. Since the current file is named `flag` and the file inside the zip file is also named `flag`, it will ask whether we want to rename the file or not. Enter `r` to rename the file to `flag-extracted`.

![image](https://github.com/encient/FSECSS-Rise-of-Kali-2023-Beginner-CTF-Writeup/assets/95013757/04c3c80a-1030-4654-8e73-ee8f892d4fdf)

Once extracted, you will get the file named `flag-extracted` (as you renamed it just now). `file flag-extracted` to see the file type. It will show that it is XZ file this time. For XZ file type, we will have to rename the file to `.xz` in order for it to be extracted. Do `mv flag-extracted flag-extracted.xz` to rename the `flag-extracted` to `flag-extracted.xz`. Then, `xz -d flag-extracted.xz` to extract the file. Once extracted, the `.xz` format will be removed.

![image](https://github.com/encient/FSECSS-Rise-of-Kali-2023-Beginner-CTF-Writeup/assets/95013757/c721c192-9d9d-44b5-822e-194043b3f0ae)

Use the same command to detect the file format. `file flag-extracted` and we will know that it is a `bz` file this time. Use `bunzip2 flag-extracted` command to extract the file. The output will then be saved as `flag-extracted.out`. `cat flag-extracted.out` to view the flag.


# Flag
`ROK{z1p_m45t3r}`
