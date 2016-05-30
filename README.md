# Linux Server Configuration

- Project can be accessed at http://52.38.72.13, port 2200
- Complete URL for hosted project: http://ec2-52-38-72-13.us-west-2.compute.amazonaws.com

#### Changes made:
  - installed updates
  - installed unattended-upgrades package to automatically manage updates for installed packages
  - created new user 'grader' with sudo permissions and diasbled root login
  - changed SSH port from 22 to 2200
  - set up firewall to only allow connections for ports 2200, 80 and 123
  - created SSH key pair
  - changed timezone configuration to UTC
  - installed apache2, git, libapache2-mod-wsgi, python-dev
  - created directory structure for catalog project
  - installed pip and virtualenv
  - imported catalog project from github and moved files into the directory structure
  - installed packages needed to run the catalog Flask application:
    - sqlalchemy, psycopg2, oauth2client, flask-seasurf, httplib2, requests, dict2xml
  - set up catalog database in virtualenv using psql
  - updated configuration catalog apache configuration file to add hostname and allow Oauth login

#### Resources used for this project:
 - compiled list of resources/walkthrough by [stueken](https://github.com/stueken/FSND-P5_Linux-Server-Configuration)
 - [Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps) [1] (https://www.digitalocean.com/community/tutorials/how-to-configure-ssh-key-based-authentication-on-a-linux-server) [2](https://www.digitalocean.com/community/tutorials/how-to-add-and-delete-users-on-an-ubuntu-14-04-vps)
 - [Ubuntu documentation (multiple pages)](https://help.ubuntu.com/)
 - [Udacity forums (multiple topics)](https://discussions.udacity.com/c/nd004-p7-linux-based-server-configuration)
 - [Stack Overflow](https://stackoverflow.com/questions/16850350/got-origin-mismatch-error-in-google-share-api) [1](https://stackoverflow.com/questions/5420789/how-to-install-psycopg2-with-pip-on-python) [2](https://stackoverflow.com/questions/15408969/how-do-i-destroy-a-vm-when-i-deleted-the-vagrant-file) [3](https://stackoverflow.com/questions/11828270/how-to-exit-the-vim-editor)
 - Udacity - [Linux Command Line Basics](https://classroom.udacity.com/nanodegrees/nd004/parts/00413454014/modules/357367901175460/lessons/4597278561/concepts/46968695970923) and [Configuring Linux Web Servers](https://classroom.udacity.com/nanodegrees/nd004/parts/00413454014/modules/357367901175461/lessons/4378692847/concepts/48114089370923)
 - http://www.hcidata.info/host2ip.cgi (Find hostname of IP address)
 - [pip documentation](https://pip.pypa.io/en/stable/reference/pip_install/)
 - [askubuntu](https://askubuntu.com/questions/172629/how-do-i-move-all-files-from-one-folder-to-another-using-the-command-line/172634)
 - [github markdown guide](https://guides.github.com/features/mastering-markdown/)
