# Reference material

## Unix Systems
#### Find Linux Files by Name or Extension
Use find from the command line to locate a specific file by name or extension. The following example searches for *.err files in the /home/username/ directory and all sub-directories:

`$ find /home/username/ -name "*.err"`

Reference: [linode](https://www.linode.com/docs/tools-reference/tools/find-files-in-linux-using-the-command-line/)

#### Search matching strings within a script
`$ cat MessageType.py | grep 13`

## Vim

* Show line numbers 
`set number`

*  Go to a line number
`123+G`
`123+gg`

* Change color scheme 
`:colorscheme [tab]`

## TMUX
* Attach to a named session
`$ tmux a -t myname`
* start new with session myname
`$ tmux new -s myname`

## Markdown preview

* Preview markdown in terminal 
`$ mdv ~/foo/bar.md`


## Python 
#### Virtual Enviornments (virtualenv)

1. Create virtual environment for a project: 
`$ cd my_projiect_folder`
`$ virtualenv my_project`

2. optional - select interpreter 
`$ virtualenv -p /usr/bin/python2.7 my_project`

3. Activate virtual environment
`$ source my_project/bin/activate` \\


###Other usefull tools
* Create a list of all the packages used
`$ pip freeze > requirements.txt` 
* install all packages from list above
`pip install -r requirements.txt`

Reference [docs.python](https://docs.python-guide.org/dev/virtualenvs/)

## Trezor Core

Location of "message type": trezor-core/src/trezor/messages/MessageType.py


## Cheet Sheets
[Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#links) 
[tmux](https://gist.github.com/MohamedAlaa/2961058)
[nano](https://www.codexpedia.com/text-editor/nano-text-editor-command-cheatsheet/)
[vim](https://vim.rtorr.com/)
