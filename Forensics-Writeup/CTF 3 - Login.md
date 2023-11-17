# Question
I have logged in into a HTTP website before, but I forgot my credentials now. Luckily, I saved the network traffic when I logged in. Can you help find my username and password?

Attachment: `login.pcapng`

Flag format: `ROK{username_password}`


# Solution
The question hints about HTTP. Therefore, we could view the HTTP data through the filter. 

`Right click` -> `Follow` -> `TCP Stream`

![[login.png]]

Then, you will see the username and password.

![[login2.png]]


# Creation
Go to a HTTP website, login and capture the network.


# Flag
`ROK{user123_sup3rs3cr3tp455}