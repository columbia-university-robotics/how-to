# How to Connect to Jetson Server

Each Jetson has a two digit ID, for example, the primary jetson has `jetson-tx2`. This tutorial will show you how to log into `jetson-tx2', the jetson that the car runs on. 

## Step 1

We need to edit the `.ssh/config` file. Please enter the following command

`vim ~/.ssh/config`

Paste the following code to the end of this file. 

    Host jetson-tx2
        ProxyJump tunnel@servers.columbiaroboticsclub.com
        Hostname localhost
        Port 43108
        ForwardX11 yes
        ForwardAgent yes
        
Close vim and save the file by pressing `Ctl + c`, and entering `:wq`

## Step 2

How you are ready to connect to the jetson. To test your setup, please enter the following command

`ssh curc@jetson-tx2`

You will be prompted to enter the tunnel password. You will be prompted to enter the public account password, which is `curc`. Once you login, the public account should automatically disconnect. If you see the message `Columbia Robotics Jetson`, then the test was successful.

## Step 3

Ask your sub-team lead to create your own user account on the Jetson.  I recommend using your uni as your username. Once your personal account has been created, you can try logging with `ssh uni@jetson-tx2`. 


## (optional) Step 4

To log into the Jetson without needing a password, do the following 2 steps:

1. Navigate to your ~/.ssh directory and run ssh-keygen
2. Then run ssh-copy-id -i (the filename of the public key) uni@jetson-tx2

Follow the prompts and you'll have the key shared with the remote server, and be able to ssh without your password (but you'll still need the tunnel password)
