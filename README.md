Version Control: keep track and manage file

version control is use to keep track of file progress

git: is a distributed version controol system that help developers track their code base and manage multiple version of a project.

github: is a remote platform use for  version control and collaboration.

git is a version control while github offers collaboration for developer.


Comprehensive git and GitHub setup for beginners.

==sudo apt update
Get:2 http://archive.ubuntu.com/ubuntu focal-updates InRelease [114 kB]
...
Reading package lists... Done


==sudo apt install git
Reading package lists... Done
Building dependency tree... Done
The following additional packages will be installed:
  git-man liberror-perl
...
Setting up git (x.xx.x) ...

==git config --global user.name "Your Name"
==git config --global user.email "your email@example.com"

To check whether your name and Email is registered successful

==user.name=Your Name
==user.email=youremail@example.com
...
To setup SSH
==ssh-keygen -t ed25519 -C "youremail@example.com"

OUTPUT

Generating public/private ed25519 key pair.
==Enter file in which to save the key (/home/user/.ssh/ided25519): [Press Enter]
==Enter passphrase (empty for no passphrase): [Press Enter]

==eval "$(ssh-agent -s)"
==ssh-add ~/.ssh/ided25519

OUTPUT
Agent pid 1234
Identity added: /home/user/.ssh/ided25519

==cat ~/.ssh/ided25519.pub

OUTPUT
ssh-ed25519 AAAAC3Nza... youremail@example.com
copy the above to your github.

