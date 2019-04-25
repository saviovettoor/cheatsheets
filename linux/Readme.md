```
Command to listout client IP of current ssh connections?
]#pinky
 or
]# echo $SSH_CLIENT
  or
]# echo $SSH_CONNECTION
```

```
Check out Client IPs connected to specific app using specific port
eg:(jenkins:8080)
]# lsof -i :8080
```
