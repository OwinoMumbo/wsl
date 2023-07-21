# Windows Subsystem Linux 
    by Shawn Mumbo, Haseeenah Sami and Kevin Naidoo
## BIOS

Before the start of this project there is a couple of settings needed to be checked on the BIOS to allow WSL and virtulization in general.
You can skip this step if you have done it before.
Restart your Pc and click the hotkey (Usuallly F2 or F10).
Enable Secure Virtulization, if you are lost on how to there is documentation below on various ways you can enable virtualization on your device.

[BIOS Settings Documentation](https://www.minitool.com/news/enable-virtualization-windows-10.html)

## Windows

### On the windows search bar, Open windows features turn on and off, turn on Windows subsystem for linux and virtual machine options.
### Open Powershell and run as admin

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
    
### Dependencies and Plugins:<br>

To update the system

      sudo apt-get update<br>

To Manage Documentatation and webview 

      sudo apt-get install libssl-dev <br>
      sudo apt-get install autoconf<br>
      sudo apt-get install libncurses5-dev<br>
      sudo apt-get install fop<br>
      sudo apt install libjpeg-dev libpng-dev libtiff-dev zlib1g-dev libncurses5-dev libssh-dev unixodbc-dev libgmp3-dev libwxbase3.0-dev libwxgtk3.0-gtk3-dev libwxgtk-webview3.0-gtk3-dev libsctp-dev lksctp-tools build-essential libgtk-3-dev libnotify-dev libsecret-1-dev catch<br>
      sudo apt install libwxgtk-webview3.0-gtk3-dev<br>
      
      sudo apt-get install xsltproc<br>
      
      sudo apt install libxml2-utils<br>

To Manage Database, Java and Python installation and their dependancies that will be used on projects

      sudo apt-get install unixodbc-dev<br>
      sudo apt install default-jdk<br>
      sudo apt-get install erlang-jinterface<br>
      sudo apt install python3 g++ make python3-pip<br>
      sudo apt install inotify-tools libtool automake libgmp-dev make libwxgtk-webview3.0-gtk3-dev libssl-dev libncurses5-dev curl git<br> 
      
Click here for [Linux Package Install Documentation](https://howtoinstall.co/en/)
And search the specified command for explanation.
      
      
   Plugins:
### We Install node Js to check if asdf is working as a package installer
    
        asdf install nodejs latest    
        asdf local nodejs latest    
        asdf global nodejs latest

        
### We Install elixir and erlang plugins 

        
        asdf plugin add erlang    
        asdf plugin add elixir

### We check for the latest version of erlang and elixir supported by ElixirLs plugin
### For the steps below please use the correct and latest version updates available on support i.e (~>"25.3.2.3"/"1.15.0-otp-25")
the update on support can be found in the link here [Elixir ls Documentation](https://github.com/elixir-lsp/elixir-ls)

        asdf list-all erlang
        KERL_BUILD_DOCS=yes asdf install erlang 25.3.2.3
        asdf list-all elixir
        asdf install elixir 1.15.0-otp-25    

### Set the envinment settings to enable the Elixir ls to work and other third party pluggins
        asdf local elixir 1.15.0-otp-25    
        asdf global elixir 1.15.0-otp-25
        asdf local erlang 25.3.2.3  
        asdf global erlang 25.3.2.3

### To check if the Elixir ls is installed properly it should return a version number.
        elixir -v




     
   
