# Question
Where words fail, music speaks.

Attachment: `music.wav`

# Solution
By using `binwalk`, we will be able to see that there is an embedded PNG file inside the mp3 file. If you use command `binwalk -e music.mp3` to extract it, you might not get the hidden file. You can try other command like `binwalk --dd="*" music.mp3` to extract all files. Finally, use `eog flag.png` to view the extracted hidden file.


# Creation
`cat file-to-show.png file-to-hide.png > output.png`
`cat music.wav flag.png > music2.wav`
`cat music-backup.mp3 flag.png > music.mp3`


# Flag
`ROK{m0r3_th4n_a_mus1c}`
