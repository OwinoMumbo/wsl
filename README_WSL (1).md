# Windows Subsystem Linux 
    by Shawn Mumbo, Haseeenah Sami and Kevin Naidoo
## BIOS



## Windows

##On the windows search bar, Open windows features turn on and off, turn on Windows subsystem for linux and virtual machine options.
##Open Powershell and run as admin

    wsl --install
    wsl --status

   Confirm it is wsl-2
   Click here for [WSL Documentation](https://learn.microsoft.com/en-us/windows/wsl/)

## Linux Terminal

### Ubuntu commands to check linux version, confirm linux installation and install git using curl to enable data transfer over various network protocols. 

    Open UBUNTU as admin
      pwd
      lsb_release -a 
      sudo apt install curl git
## Package Handler:

### This installs asdf package handler. 

    git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.12.0     
    echo ". $HOME/.asdf/asdf.sh" >> ~/.bashrc     
    source ~/.bashrc
    asdf plugin add nodejs https://github.com/asdf-vm/asdf-nodejs.git\
Click here for [asdf Documentation](https://asdf-vm.com/guide/introduction.html)
    
Dependencies and Plugins:
      sudo apt-get update
      sudo apt-get install libssl-dev
      sudo apt-get install autoconf
      sudo apt-get install libncurses5-dev 
      sudo apt-get install fop 
      sudo apt install python3 g++ make python3-pip 
      sudo apt-get install xsltproc 
      sudo apt-get install unixodbc-dev
      sudo apt install libxml2-utils
      sudo apt install default-jdk
      sudo apt-get install erlang-jinterface
      sudo apt install inotify-tools libtool automake libgmp-dev make libwxgtk-webview3.0-gtk3-dev libssl-dev libncurses5-dev curl git 
      sudo apt install libjpeg-dev libpng-dev libtiff-dev zlib1g-dev libncurses5-dev libssh-dev unixodbc-dev libgmp3-dev libwxbase3.0-dev libwxgtk3.0-gtk3-dev libwxgtk-webview3.0-gtk3-dev libsctp-dev lksctp-tools build-essential libgtk-3-dev libnotify-dev libsecret-1-dev catch  
      sudo apt install libwxgtk-webview3.0-gtk3-dev
Click here for [Linux Package Install Documentation](https://howtoinstall.co/en/)
And search the specified command for explanation.
      
      
   Plugins:
###We Install node Js to check if asdf is working as a package installer
    
        asdf install nodejs latest    
        asdf local nodejs latest    
        asdf global nodejs latest

        
###We Install elixir and erlang plugins 

        
        asdf plugin add erlang    
        asdf plugin add elixir

        
        asdf list-all erlang
        KERL_BUILD_DOCS=yes asdf install erlang 25.3.2.3       
        asdf install elixir 1.15.0-otp-25    

         
        asdf local elixir 1.15.0-otp-25    
        asdf global elixir 1.15.0-otp-25
        asdf local erlang 25.3.2.3  
        asdf global erlang 25.3.2.3    
        elixir -v




     
   
