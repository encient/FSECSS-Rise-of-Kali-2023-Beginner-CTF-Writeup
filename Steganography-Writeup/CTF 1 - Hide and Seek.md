# Question
I have hidden a message in this image, but I forgot the passphrase. Can you help me to uncover the message?

Attachment: `image.jpg`


# Solution
The question says that something is hidden in the file but with unknown password. Normally tools like `steghide` can hide a message while using a password to secure it. Therefore, we can try to search for password bruteforce tool. The challenge title and image show about hide and seek, so upon searching in the internet, you will be able to find a tool called [stegseek](https://github.com/RickdeJager/stegseek). Download the tool and use it to bruteforce the password. The wordlist that we normally use for password cracking is `rockyou.txt`. If you do not have the wordlist in your machine, you can find it in internet and download it.

```
stegseek image.jpg /usr/share/wordlists/rockyou.txt
```

By using the command above, the password that will be shown is `rayofsunshine`, and it will automatically extract the embedded file `flag.txt` for you. Use `cat` command to read the `flag.txt` file to get the flag.


# Flag
`ROK{st3gh1d3_cr4ck3r}`
