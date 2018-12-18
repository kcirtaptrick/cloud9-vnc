VNC
===

Running X11 in a Cloud9 workspace.

![Screen Shot](screenshot.png)

Installation
------------


Clone the repository to where you'd like (in the example I use the home folder ~)
    
    
    cd ~
    git clone https://github.com/kcirtaptrick/cloud9-vnc.git
    

Enter the repository sub-directory

    cd cloud9-vnc/

Now make sure apt-get has been updated with 

    sudo apt-get update

Run the install script with privileges

    sudo ./install.sh

If you get the error: 
    sudo: ./install.sh: command not found
run:
    Sudo chmod a+x install.sh    
then try again


(Optional) Clean up installation directory
    
    rm -rf ./

Uninstallation
--------------

Run the uninstallation script with privileges

        sudo /opt/c9vnc/uninstall.sh
    

Running
-------

Use the custom C9 runner

    Run > Run With > C9vnc
    
Run the start script symlinked into your /usr/local/bin
    
    c9vnc

If you get the error: 
    sudo: /opt/c9vnc/c9vnc.sh: command not found
run:
    Sudo chmod a+x /opt/c9vnc/c9vnc.sh   
then try again