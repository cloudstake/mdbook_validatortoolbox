---
## Here's the breakdown of how things work to help you work with our process
---

# Things to know about our setup & process

Here's a full rundown of what happens, regular node operators should be very familiar with the process.

## Standard Signing Validating Node

For a standard node on express mode you'll be asked to setup a wallet password and import your mnemonic phrase into the hmy application directly. We build an environment variables file located at ~/.easynode.one to store our values.

We do pass your password into a file called ~/harmony/passphrase.txt which is where autobidder also requires you to store your wallet password for our usage.

At this time, only claiming rewards requires use of your passphrase but down the road we may implement more features that take advantage of this.

We are working on salted storage of passwords for people who do not utilize autobidder.

## Volumes - Additional Storage

At this point here's how storage works for our application

1. We check /mnt for a folder - If one exists we make a folder inside of that named harmony, symlink it to ~/harmony and install your files there. It's not "smart" at this point so you may need to verify your folder contents before running the installer. 
2. If you have no folders in /mnt - We set up harmony at ~/harmony in a folder. Everything else will be setup to utilize this folder for your application.

