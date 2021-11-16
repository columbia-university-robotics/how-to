# How to create a new user on the Jetson

## Prerequisite

This tutorial is for admin user's only. If you are not an admin is tutorial is not applicable. Please contact Neil or your team lead. 

## Step 1

Log in to the admin account

## Step 2

Create the user by entering

`sudo useradd -m -s /bin/bash [username]`

The username should be your UNI

## Step 3

Now we need to set the password for the new user. 

`sudo passwd [username]`

This commmand will prompt you to enter the password for the new user. 

## Step 4

Now you are ready to test the new account. You can use ssh to login to your new account, for example, `ssh yn2376@jetson-00`. By entering your password, you should be able to login to the Jetson. 

## Questions

Please contact Neil directly if you have questions. 
