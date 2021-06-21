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
* Just a command runner  https://github.com/casey/just
* pueue: Manage your shell commands https://github.com/Nukesor/pueue


### commands

* exa: modern replacement for ls https://the.exa.website/
* lsd: The next gen ls command https://github.com/Peltoche/lsd
* ack: a tool like grep, optimized for programmers https://beyondgrep.com/
* ag: A code-searching tool similar to ack, but faster https://github.com/ggreer/the_silver_searcher
* mtr : A command which is a combination of ‘ping’ and ‘traceroute’ command.
* tldr: Simplified and community-driven man pages https://github.com/tldr-pages/tldr
* nl : Outputs the content of text file with lines Numbered
* tree : Prints files and folders in tree like fashion, recursively
* broot: A new way to see and navigate directory trees https://github.com/Canop/broot
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
* git-quick-stats:  https://github.com/arzzen/git-quick-stats
* moro: Simple CLI tool for tracking work hours https://github.com/albacoretuna/moro
* taskwarrior: manages your TODO list from the command line brew install task  https://taskwarrior.org/

### File & directory

* rip (Rm ImProved) https://github.com/nivekuil/rip 
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
* cargo-make: Rust task runner and build tool  https://github.com/sagiegurari/cargo-make
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
* ncdu: ncduis a disk utility for Unix systems

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
* direnv – unclutter your .profile  https://direnv.net/

### system

* Mac App Store command line interface https://github.com/mas-cli/mas
* Swiss Army Knife for macOS: https://github.com/rgcr/m-cli
* SQL powered operating system instrumentation, monitoring, and analytics: https://osquery.io/
* command-line system information tool: https://github.com/dylanaraps/neofetch
* A terminal based graphical activity monitor inspired by gtop and vtop: https://github.com/cjbassi/gotop 
* BitBar: Put anything in your Mac OS X menu bar https://getbitbar.com/
* Beautiful calculator app for Mac: https://numi.app/ 
* procs: modern replacement for ps https://github.com/dalance/procs
* pier: A Linux script management CLI https://github.com/pier-cli/pier
* Scriptisto:  language-agnostic "shebang interpreter" that enables you to write scripts in compiled languages  https://github.com/igor-petruk/scriptisto
* hyperfine: command-line benchmarking tool  https://github.com/sharkdp/hyperfine
* sd: Intuitive find & replace CLI (sed alternative)   https://github.com/chmln/sd 
* ytop and bottom: https://github.com/cjbassi/ytop https://github.com/ClementTsang/bottom

### tools

* Taskworrior: manages your TODO list from the command line  https://taskwarrior.org/
* Timewarrior: tracks time from the command line https://timewarrior.net/

### Code

* Source-highlight: https://www.gnu.org/software/src-highlite/source-highlight.html 
* gitignore:  https://www.gitignore.io/ 
* tokei: https://github.com/XAMPPRocky/tokei
* gitui: terminal-ui for git https://github.com/extrawurst/gitui
* git-stats: https://github.com/IonicaBizau/git-stats

### Rust


### oh-my-zsh

alias -s rb=vim #opens ruby files in vim

### database

* CLI for SQLite Databases with auto-completion and syntax highlighting: https://github.com/dbcli/litecli 

### CLI frameworks

* Go: Cobra, cli
* Node: oclif, Commander.js clap.js
* Deno: yargs , cmd
* Python: Click, Typer
* Ruby: TTY, commander, GLI
* PHP: console
* Java: Picocli, JCommander, Clikt
* Rust: clap-rs, pico-args, paw
* C++: gflags, cli, docopt.cpp


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

### Shell

* The Ultimate Programmer’s Guide to Bash Scripting: https://medium.com/better-programming/the-ultimate-programmers-guide-to-bash-scripting-2d11d4e6e978
* 27 Simple Bash Scripting Tips for Beginners: https://medium.com/better-programming/27-simple-bash-scripting-tips-for-beginners-d6764c977546
* pure bash bible: https://github.com/dylanaraps/pure-bash-bible
* 13 Fantastic Learning Tools and Resources for Bash Scripting: https://medium.com/better-programming/13-fantastic-learning-tools-and-resources-for-bash-scripting-51a6de98015c

### references

* Modern Unix: https://github.com/ibraheemdev/modern-unix
* Awesome Alternatives in Rust: https://github.com/TaKO8Ki/awesome-alternatives-in-rust
* How to Set Up Your MacBook for Web Development in 2020: https://medium.com/better-programming/setting-up-your-mac-for-web-development-in-2020-659f5588b883
* The Art of Command Line https://github.com/jlevy/the-art-of-command-line
* awesome-shell: https://github.com/alebcay/awesome-shell
* github bash topic: https://github.com/topics/bash
* Mac setup: https://github.com/ptb/mac-setup
* dotfiles: https://github.com/mathiasbynens/dotfiles
* https://remysharp.com/2018/08/23/cli-improved
* Writing a Command Line Tool in Rust https://mattgathu.github.io/writing-cli-app-rust/
* 5 Tips for Writing Small CLI Tools in Rust https://deterministic.space/rust-cli-tips.html
* Command-line tools written in Rust https://www.reddit.com/r/rust/comments/70b74a/commandline_tools_written_in_rust/
* Delete Files Older Than X: https://www.baeldung.com/linux/delete-files-older-than
* Most Useful Command Line Tools: 50 Cool Tools to Improve Your Workflow, Boost Productivity, and More: https://stackify.com/top-command-line-tools/
* The Ultimate Guide to Your Terminal Makeover: https://towardsdatascience.com/the-ultimate-guide-to-your-terminal-makeover-e11f9b87ac99
* 7 Awesome Rust-powered Command-line Utilities: https://towardsdatascience.com/awesome-rust-powered-command-line-utilities-b5359c38692
* Command Line Interface Guidelines: https://clig.dev/
* 12 Factor CLI Apps: https://medium.com/@jdxcode/12-factor-cli-apps-dd3c227a0e46
* The netcat Command in Linux: https://www.baeldung.com/linux/netcat-command

