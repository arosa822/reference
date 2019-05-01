# Reference material
______
## flask
* import flask app
`$ export FLASK_APP=foo.py`
## Unix Systems
* Find Linux Files by Name or Extension
`$ find /home/username/ -name "*.err"`
* Change color of address displayed
`$ export PS1='\[\033[0;35m\]\h\[\033[0;33m\] \w\[\033[00m\]: '`
* Search matching strings within a script
`$ cat MessageType.py | grep 13`
* show processes runing on ports
`$ netstat -tulpn`
	* In order to show specific processes for other users use "sudo"
	* add `| grep <123>` to search for specific string 
* make bash script executable 
`$ chmod u+x ./foo/bar`

* unzip .tar.gz
`$ tar xvzf file.tar.gz`
* shorten the bash prompt from the command line
`$ PROMPT_DIRTRIM=1`

* create a alias for sudo // needed when "command not found"
`alias mysudo='sudo -E env "PATH=$PATh"'`
______
## Bash shortcuts
* Move to the beggining of a line: ` ctrl + a`
* Move to the end of a line: `ctrl + E ` 
* Copy output of bash to clipboard: `$ pwd | cb `
______

## Vim
* Show line numbers 
`:set number`
* Remove line numbers
`:set nonumber`
* Go to a line number
`:123+G`
`:123+gg`
* Change color scheme 
`:colorscheme [tab]`
* move to the begining of the line 
`0`
* move to the end of a line 
`$`
* show name of file
`:set laststatus=2`

* Cursor movement 
	* Up `k`
	* Down `j`
	* Left `h`
	* Right `l` 

* Undo: `u`
* Redu: `ctrl + r`
* Location of vimrc file: `/usr/share/vim/vimrc`
______
## TMUX

* Attach to a named session
`$ tmux a -t myname`
* start new with session myname
`$ tmux new -s myname`
* Enable scrolling 
`<ctrl+b> + <[>`
	* Quit scroll mode 
`q`
* Resizing pane 
`<ctrl+ b > + :` then `-<D,U,L,R>` followed by a number
	* Example: `:resize-pane -R 10`
* Reloading tmux config
   * From within tmux: `:source-file ~/.tmux.conf`
   * From a shell: `tmux source-file ~/.tmux.conf`
#### Sessions
* list sessions `ls`
* name session `$`
* kill a session `$ tmux kill-session -t myname`
* Detatch from session `ctrl+b + d`
#### Windows
* Create a new window: `c`
* Rename a window: `,`
* Show all windows: `w`
* kill a window `&`

## Markdown preview

* Preview markdown in terminal 
`$ mdv ~/foo/bar.md`
______
## Restview
restview is a tool for viewing .rst files<br/>

* installing restview
`$ pip install restview`
* using restview
`$ restview ./foo/bar.rst`

## Python 
#### Virtual Enviornments (virtualenv)

1. Create virtual environment for a project: 
`$ cd my_projiect_folder`
`$ virtualenv my_project`

2. optional - select interpreter 
`$ virtualenv -p /usr/bin/python2.7 my_project`

3. Activate virtual environment
`$ source my_project/bin/activate` \\
______

###Other usefull tools
* Create a list of all the packages used
`$ pip freeze > requirements.txt` 
* install all packages from list above
`pip install -r requirements.txt`
* view serial stream 
`$ screen /dev/ttyUSB0 115200`
______
## Trezor Core

* Location of "message type": trezor-core/src/trezor/messages/MessageType.py
* Unit tests
	* Navigate to ~/trezor-core/tests
	* `$ ../build/unix/micropython -O test_trezor.config.py`
______
## Monitor Serial 
* quick listen
`$ cat /dev/ttyUSB0`
* interactive session
`$ screen /dev/ttyUSB0 115200`
* terminate all screen sessions
`killall screen`

______
## SSH / SCP 
* Transfer files from local to remote
`$ sudo scp ./foo user@remote:/foo/bar`

______
## appium
* find appPackage and appActivity
1. `sudo adb devices`
2. `adb shell`
3. `dumpsys window windows | grep -E 'mCurrentFocus'`
______
## Cheet Sheets
[Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#links) 
[tmux](https://gist.github.com/MohamedAlaa/2961058)
[nano](https://www.codexpedia.com/text-editor/nano-text-editor-command-cheatsheet/)
[vim](https://vim.rtorr.com/)
