# command-tips


### commands

* exa: modern replacement for ls https://the.exa.website/
* ack: a tool like grep, optimized for programmers https://beyondgrep.com/
* mtr : A command which is a combination of ‘ping’ and ‘traceroute’ command.
* tldr: Simplified and community-driven man pages https://github.com/tldr-pages/tldr
* nl : Outputs the content of text file with lines Numbered
* tree : Prints files and folders in tree like fashion, recursively
* Pstree : Prints running processes with child processes, recursively
* lsof -iTCP:80 -sTCP:LISTEN. The script, outputs all the service/process using port 80.

### Network

* curl ifconfig.me : Shows machine’s external IP Address

### Files

* find . -size +100M : find fine bigger than 100M

### Services 

* Echo Service: 
```
socat -v tcp-l:1234,fork exec:'/bin/cat'
```
* simple web server for the current directory
```
Python -m SimpleHTTPServer
```
* A simple development http server with live reload https://github.com/tapio/live-server
```
npx live-server
```
### Funny

* cowsay: cowsay is a configurable talking cow https://github.com/piuccio/cowsay
* toilet: Colored Text
* watch -t -n1 "date +%T|toilet"