# Question
Extract the all the files to get the flag.

Attachment: `flag`

# Solution
This challenge is for you to learn how to extract different types of zip files. However, the file does not show what is the file type. Therefore, we have to use `file` command to determine the file type. Below are the steps to solve this challenge: 

`file flag`
`unzip flag`
`file flag`
`mv flag flag.xz`
`xz -d flag.xz`
`file flag`
`bunzip2 flag`
`cat flag.out`


# Creation
`nano flag.txt`
`bzip2 flag.txt`
`mv flag.txt.bz2 flag`
`xz flag`
`mv flag.xz flag`
`zip -r flag flag`


# Flag
`ROK{z1p_m45t3r}`