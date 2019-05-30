# command-tips


### Structures 
dotfiles & script

* .aliases: https://github.com/sebglazebrook/aliases 
* .aliases_legacy: tranditional alias
* .functions: custom functions
* .exports: export
* .sources: sources
* brew.sh: install brew artifacts
* .justfile/justfile-java:  justfile for java
* bootstrap.sh: for bootstrap

### shell

* Bash Automated Testing System https://github.com/sstephenson/bats

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
* Public URLs to internet from local: https://ngrok.com/
* A terminal UI for tshark, inspired by Wireshark: https://github.com/gcla/termshark

### Kubernetes

* Fast way to switch between clusters and namespaces in kubectl https://github.com/ahmetb/kubectx 

### Productivity

* Git extras: https://github.com/tj/git-extras

### File & directory

* find . -size +100M : find fine bigger than 100M
* gshred or srm: Delete File Permanently 
* Watch Logs in Real-Time
```
watch tail /var/log/auth.log
```
* watchman: A file watching service https://facebook.github.io/watchman/
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
* jq: lightweight and flexible command-line JSON processor https://stedolan.github.io/jq/
* fx: Terminal JSON viewer https://github.com/antonmedv/fx
* Monitor a process and trigger a notification https://github.com/variadico/noti
* Run arbitrary commands when files change: http://www.entrproject.org
* Make JSON greppable: https://github.com/TomNomNom/gron 
* A cd command that learns - easily navigate directories from the command line  https://github.com/wting/autojump
* tig: https://jonas.github.io/tig/doc/tig.1.html
* fasd: Command-line productivity booster, offers quick access to files and directories, inspired by autojump, z and v. https://github.com/clvv/fasd
* Find files with SQL-like queries: https://github.com/jhspetersson/fselect
* An advanced log file viewer for the small-scale http://lnav.org/
* hexyl: A command-line hex viewer https://github.com/sharkdp/hexyl
* Command line text processing: https://github.com/learnbyexample/Command-line-text-processing

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
* termtosvg: Record terminal sessions as SVG animations  https://github.com/nbedos/termtosvg

### system

* Mac App Store command line interface https://github.com/mas-cli/mas
* Swiss Army Knife for macOS: https://github.com/rgcr/m-cli
* SQL powered operating system instrumentation, monitoring, and analytics: https://osquery.io/
* command-line system information tool: https://github.com/dylanaraps/neofetch
* A terminal based graphical activity monitor inspired by gtop and vtop: https://github.com/cjbassi/gotop 

### oh-my-zsh

alias -s rb=vim #opens ruby files in vim

### database

* CLI for SQLite Databases with auto-completion and syntax highlighting: https://github.com/dbcli/litecli 

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

* The Art of Command Line https://github.com/jlevy/the-art-of-command-line
* awesome-shell: https://github.com/alebcay/awesome-shell
* github bash topic: https://github.com/topics/bash
* Mac setup: https://github.com/ptb/mac-setup
* dotfiles: https://github.com/mathiasbynens/dotfiles
* https://remysharp.com/2018/08/23/cli-improved
* Writing a Command Line Tool in Rust https://mattgathu.github.io/writing-cli-app-rust/
* 5 Tips for Writing Small CLI Tools in Rust https://deterministic.space/rust-cli-tips.html
* Command-line tools written in Rust https://www.reddit.com/r/rust/comments/70b74a/commandline_tools_written_in_rust/
