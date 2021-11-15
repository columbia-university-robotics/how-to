# How to Connect to Jetson Server

Each team will have a different device (Jetson). Each Jetson has a two digit ID, for example, the computer vision team of the autonomous vehicles project has `jetson-00`. This tutorial will show you how to log into `jetson-00`

## Step 1

We need to edit the `.ssh/config` file. Please enter the following command

`vim .ssh/config`

Paste the following code to the end of this file. 

    Host jetson-00
        ProxyJump tunnel@servers.columbiaroboticsclub.com
        Hostname localhost
        Port 43100
        ForwardX11 yes
        ForwardAgent yes
        
Close vim and save the file by pressing $Ctl + c$, and entering `:wq`

## Step 2

How you are ready to connect to Jetson 00. Please enter the following command

`ssh curc-public@jetson-00`

You will be prompted to enter the tunnel password. You will be prompted to enter the public account password, which is `curc`. Once you login, the public account should automatically disconnect. If you see the message `Columbia Robotics Jetson 00`, then the test was successful.

## Step 3

Ask your sub-team lead to create your own user account on the Jetson.  I recommend using your uni as your username. Once your personal account has been created, you can try logging with `ssh uni@jetson-00`. 
