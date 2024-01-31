# Chat Server Explained
See the server in action as well as an explanation of what is happening. 
![image](firstPersonTalm)
In this image you can see the use of the url in order to send a message along with you username into the website. 
The code takes the url and splits it into two parts at the "&" sign leaving "s=helloo" and "user=person1".
It then splits the two parts at the "=" sign resulting in "s" and "helloo" in one and "user" and "person1" in the other.
The results are placed into two arrays, one for usernames and the other for messages. Within in both arrays the items at index 0 are the parts on the left of the "=" and the index 1 is the right side. Example: user has {user, person1}
We take the items at index 1 and use them as arguments so we can format them as <user>: <message> and return this result. We also add this result to a String called "Chatlogs" that takes this same format and puts a "\n" so that all messages are placed on a new line. The website itself displays the Chatlogs String.
Methods called: handleRequest(), getPath(), contains(), getQuery(), split(), format().
Relevant Arguments: url used in handleRequest() and  getPath(), "/add-message"  and "s" used in contains(), "&" and "=" used in split(), user[1] and  message[1] used in format()
Values Changed: the url changes, the arguments for user and message arrays change, and the Chatlogs string is updated with the message and user.
