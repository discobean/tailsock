# tailsock
A simple one file tail app that lets you tail files in your web browser.  It can also show a glob pattern match.

Usage:
````
$ pip install -r requirements.txt
$ ./tailsock
Usage: ./tailsock [-p <port>] [-n <num>] -f <file/dir/glob>
       -p <port> : specify port number, default random
       -n <num>  : number of rows to show initially, default 200
````

Examples:
````
$ ./tailsock -f test.log
http://192.168.178.24:55979

$ ./tailsock -f '/logs/*.log'
http://192.168.178.24:55979
````
Then visit the URL shown in your browser and watch the magic happen, tested in Chrome.
