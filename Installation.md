1. To install Hyperledger on Ubuntu 18.04, follow these steps:\
        $ sudo apt-get update

2. Install curl and the golang software package:\
        $ sudo apt-get install curl\
        $ sudo apt-get install golang\
        $ export GOPATH=$HOME/go\
        $ export PATH=$PATH:$GOPATH/bin

3. Install Node.js, npm, and Python:\
        $ sudo apt-get install nodejs\
        $ sudo apt-get install npm\
        $ sudo apt-get install python

4. Install and upgrade docker and docker-compose:\
        $ sudo apt-get install docker\
        $ curl -fsSL https://download.docker.com/linux/ubuntu/gpg |      
          sudo apt-key add -\
        $ sudo add-apt-repository "deb [arch=amd64]   
          https://download.docker.com/linux/ubuntu 
        $(lsb_release -cs) stable"\
        $ sudo apt-get update\
        $ apt-cache policy docker-ce\
        $ sudo apt-get install -y docker-ce\
        $ sudo apt-get install docker-compose\
        $ sudo apt-get upgrade
        
5. Let's customize and update Node.js and golang to the proper versions:\
        $ wget https://dl.google.com/go/go1.11.2.linux-amd64.tar.gz \
        $ tar -xzvf go1.11.2.linux-amd64.tar.gz\
        $ sudo mv go/ /usr/local\
        $ export GOPATH=/usr/local/go\
        $ export PATH=$PATH:$GOPATH/bin\
        $ curl -sL https://deb.nodesource.com/setup_8.x | sudo bash -\
        $ sudo apt-get install -y nodejs

6. Verify the installed software package versions:\
        $ curl --version\
        $ /usr/local/go/bin/go version\
        $ python -V\
        $ node -v\
        $ npm -version\
        $ docker --version\
        $ docker-compose --version
        
 7. Install Hyperledger Fabric 1.3:\
         $ curl -sSL http://bit.ly/2ysbOFE | sudo bash -s 1.3.0
         
 
