Bootstrap: docker
From: godlovedc/lolcow:latest

%runscript
    echo
    echo ===============================================
    echo Attempting to install lolcow in ~/lolcow
    echo ===============================================
    echo

    if [ -d "/home/$USER/lolcow" ]; then 
         echo "~/lolcow already exists"
         echo "will not overwrite"
         echo
         exit 1
    fi
  
    mkdir ~/lolcow
    cp -r GodloveD-lolcow-installer-master.img ~/lolcow/image

    cd ~/lolcow
    cat > lolcow.sh <<"EOF"
#!/bin/bash
# if you want to bind some host directories...
# export SINGULARTY_BINDPATH=/some,/dirs,/to,/bind
dir=$(dirname  "$0")
cmd=$(basename "$0")
arg="$@"
singularity exec $dir/image $cmd $arg
EOF
    
    chmod 755 lolcow.sh

    ln -s lolcow.sh fortune
    ln -s lolcow.sh cowsay
    ln -s lolcow.sh lolcat

    cowsay 'type "export PATH=~/lolcow:$PATH" and enjoy fortune, cowsay, and lolcat!' |\
    lolcat
