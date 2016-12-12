# tailsock
A simple one file tail app that lets you tail files in your web browser

Usage:
    $ ./tailsock
    Usage: ./tailsock [-p <port>] [-n <num>] [-o] -f <filename>
       -p <port> : specify port number, default random
       -n <num>  : number of rows to show initially, default 50
       -o        : oneshot, exits once browser is closed, default off

Example:

    $ ./tailsock -f test.log
    http://192.168.178.24:55979

Then visit the URL shown in your browser and watch the magic happen, tested in Chrome.
