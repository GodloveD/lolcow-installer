# lolcow-installer

## Step 0: install [Singularity](https://github.com/singularityware/singularity)

[This](http://singularity.lbl.gov/docs-quick-start-installation) will help.

## Step 1: run `lolcow-installer` from Singularity Hub

```
[dave@hal2001:~]$ singularity run shub://GodloveD/lolcow-installer
Progress |===================================| 100.0% 

===============================================
Attempting to install lolcow in /home/dave/lolcow
===============================================

 _______________________________________
/ type "export PATH=~/lolcow:$PATH" and \
\ enjoy fortune, cowsay, and lolcat!    /
 ---------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```

## Step 2: Do as the cow commands

```
[dave@hal2001:~]$ export PATH=~/lolcow:$PATH

```

## Step 3: Enjoy computer fun
```
[dave@hal2001:~]$ fortune | cowsay | lolcat 
 ____________________________________
/ Q: What is orange and goes "click, \
\ click?" A: A ball point carrot.    /
 ------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```

<i>Ha ha ha!<\i>
