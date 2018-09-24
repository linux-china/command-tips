# command-tips


### commands

* exa: modern replacement for ls https://the.exa.website/
* ack: a tool like grep, optimized for programmers https://beyondgrep.com/
* ag: A code-searching tool similar to ack, but faster https://github.com/ggreer/the_silver_searcher
* mtr : A command which is a combination of ‘ping’ and ‘traceroute’ command.
* tldr: Simplified and community-driven man pages https://github.com/tldr-pages/tldr
* nl : Outputs the content of text file with lines Numbered
* tree : Prints files and folders in tree like fashion, recursively
* Pstree : Prints running processes with child processes, recursively
* lsof -iTCP:80 -sTCP:LISTEN. The script, outputs all the service/process using port 80.
* htop:  an interactive process viewer for Unix https://hisham.hm/htop/
* Glances an Eye on your system. A top/htop alternative https://github.com/nicolargo/glances
* direct normal output and errors to /dev/null
```
xxxxx  > /dev/null 2>&1
```
### Network

* curl ifconfig.me : Shows machine’s external IP Address
* get primary ip
```
ifconfig | grep -Eo 'inet (addr:)?([0-9]*\.){3}[0-9]*' | grep -Eo '([0-9]*\.){3}[0-9]*' | grep -v '127.0.0.1'
```
* ApacheBench (ab) replacement: https://github.com/rakyll/hey

### File & directory

* find . -size +100M : find fine bigger than 100M
* gshred or srm: Delete File Permanently 
* Watch Logs in Real-Time
```
watch tail /var/log/auth.log
```
* A cat(1) clone with wings.  https://github.com/sharkdp/bat brew install 
* A program that allows you to count your code, quickly. cloc replacement https://github.com/Aaronepower/tokei 
* fd is a simple, fast and user-friendly alternative to find.  https://github.com/sharkdp/fd 
* ripgrep recursively searches directories for a regex pattern  https://github.com/BurntSushi/ripgrep 
* Project templates in rust https://github.com/vmchale/project-init
* Just a command runner  https://github.com/casey/just
* A fast CSV command line toolkit written in Rust. https://github.com/BurntSushi/xsv
* Executes commands in response to file modifications https://github.com/watchexec/watchexec
* command-line fuzzy finder:  https://github.com/junegunn/fzf  
```
alias preview="fzf --height 40% --preview 'if file -i {}|grep -q binary; then file -b {}; else bat --color \"always\" --line-range :40 {}; fi'"
```
* fastest terminal file manager  https://github.com/jarun/nnn
* jq: https://stedolan.github.io/jq/
* Monitor a process and trigger a notification https://github.com/variadico/noti
* Run arbitrary commands when files change: http://www.entrproject.org
* Make JSON greppable: https://github.com/TomNomNom/gron 
* A cd command that learns - easily navigate directories from the command line  https://github.com/wting/autojump
* tig: https://jonas.github.io/tig/doc/tig.1.html
* fasd: Command-line productivity booster, offers quick access to files and directories, inspired by autojump, z and v. https://github.com/clvv/fasd
* Find files with SQL-like queries: https://github.com/jhspetersson/fselect
* An advanced log file viewer for the small-scale http://lnav.org/

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

### oh-my-zsh

alias -s rb=vim #opens ruby files in vim


### Funny

* cowsay: cowsay is a configurable talking cow https://github.com/piuccio/cowsay
* toilet: Colored Text
* lolcat: Rainbows and unicorns!
* watch -t -n1 "date +%T|toilet"
* look: Check for Spelling of Words in Linux 
* say: english words pronounce

### Books

* http://conqueringthecommandline.com/book
* Data Science at the Command Line https://www.datascienceatthecommandline.com/


### references

* https://remysharp.com/2018/08/23/cli-improved
* Writing a Command Line Tool in Rust https://mattgathu.github.io/writing-cli-app-rust/
* 5 Tips for Writing Small CLI Tools in Rust https://deterministic.space/rust-cli-tips.html
* Command-line tools written in Rust https://www.reddit.com/r/rust/comments/70b74a/commandline_tools_written_in_rust/