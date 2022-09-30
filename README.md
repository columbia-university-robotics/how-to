# How to...

This repo contains short documentation and tutorials on various software packages and tools that we use. 

## Contact

Please message Tameem (tma2153[at] columbia.edu) and or Justin (jc5525[at] columbia.edu) directly if you have any questions.

## Contributing

First do these two steps to enable your computer to connect to Git as your user:
[First set up an ssh key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
[Then pair it to Git](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
To contribute to a CURC repo, perform the following steps: 

First clone the repo you wish to contribute to (self driving, in this example):
    git clone git@github.com:columbia-university-robotics/self-driving-car.git

Then, open a new branch for your changes:
    git checkout -b {yourName}/{yourChange}

Then, work on your changes, and when you're done, do:
    git add {files you changed}
    git commit -m "put details of your change in these quotes"

When you finish testing your work, do:
    git push origin HEAD
and if prompted, follow the link provided in the terminal. 