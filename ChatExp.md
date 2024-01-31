# Chat Server Explained
See the server in action as well as an explanation of what is happening. 
---
![image](firstPersonTalm)
**Methods called:** `handleRequest(), getPath(), contains(), getQuery(), split(), format().`\
**Relevant Arguments:** url used in `handleRequest()` and  `getPath()`.  "/add-message"  and "s" used in `contains()`. "&" and "=" used in `split()`. user[1] and message[1] used in `format()`\
**Values Changed:** the url changes, the arguments for `user` and `message` arrays change to "person1" and "helloo", and the `Chatlogs` string is updated with the message and user "person1: helloo \n".
![image](2ndtalmer)
**Methods called:** `handleRequest(), getPath(), contains(), getQuery(), split(), format().`\
**Relevant Arguments:** url used in `handleRequest()` and  `getPath()`.  "/add-message"  and "s" used in `contains()`. "&" and "=" used in `split()`. user[1] and message[1] used in `format()`\
**Values Changed:** the url changes, the arguments for `user` and `message` arrays change to "individual2" and "hiii", and the `Chatlogs` string is updated with the message and user "individual2: hiii \n".
![image](finalchat)
`Chatlogs` is displayed as the website is viewed with no query in the url allowing you to see all messages sent.\
\
[Back to Web Server Code](chatServer.md)
