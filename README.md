##How to learn your bash shell to whisper previous commands

 - copy the file ***.inputrc*** into your home directory (like */home/jaroslav/*).
 - restart you bash by simple re-login; or better, by restarting bash itself
 ```
 exec bash -l
 ```
 
###Result
Any command you ever wrote to shell can be simply restored by write part of it and pressing **up arrow**.

####Example
You connected via a ssh tunnel to remote MySQL database yesterday
```
ssh -Ng -L 15000:localhost:3306 production-server-1
```

And today, you want to do the same. Just write
```
ssh -
```
and press *up arrow*. Voala, your yesterday command reveals.

Keep pressing the *up arrow* to list over all similar commands, written sometime in history, starting by ```ssh -``` string.
