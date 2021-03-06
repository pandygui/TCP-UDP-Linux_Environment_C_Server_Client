# Owner: Daniel Better
## An implementation of a Server/Client application based on both TCP/UDP protocols

How to run the client/server:

There's a "Makefile" included in the folder of the excercise.
```
Make
```

After "Make", there'll be 2 executable files, "server" & "client".

### First of all, activate the "server":
There are two options as to how to run the server:


**TCP connection**, supports -d & -s flags
  * -d for directive to start at
  * -s for "select" implementation of the new connections instead of "fork"
```
$./server
```
**UDP connection**, also supports the -d directive.
```
$./server -u
```


when server is activated with -u the client must be run with -u corressponding aswell (instructions up-ahead)

### Now we can run the client: 2 options:
**TCP connection:**
```
$./client 127.0.0.1
``` 
**UDP connection:** (must be corressponding to the $./server -u option)
```
$./client 127.0.0.1 -u
```

The client supports the following commands: cd, lcd, put, get, dir, quit. 