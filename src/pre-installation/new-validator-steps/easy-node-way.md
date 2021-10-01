# The "validatortoolbox" Way of Harmony Server Installation
---
Here's a full rundown of what happens, regular node operators should be very familiar with the process.

## Location
We install your files in your users home directory in ~/harmony
- If you use a volume to store your data, mount it in /mnt/[ANY_FOLDER] and we will install in /mnt/[ANY_FOLDER]/harmony and symlink back to ~/harmony
- This allows nothing else other than your file storage location to change. You can still run & edit everything as per usual in ~/harmony

## Variables
We create a file named ~/.easynode.env to store the info you pick on our menus

## Wallet & Wallet Password
If you choose a Standard Wallet Node you'll put your mnemonic phrase directly into the hmy interface - We do not pass through or store your mnemonic phrase. Your wallet password is also saved to ~/harmony/passphrase.txt for use later with our menu applicaton & autobidder (if installed).

## Volumes - Additional Storage
At this point here's how storage works for our application
- We check for a volume.
- We check /mnt for a single volume mounted to a folder.
    - If one exists we make a folder inside of that named harmony, symlink it to ~/harmony and install your files there.
    - If you have no folders in /mnt - We set up harmony at ~/harmony in a folder. Everything else will be setup to utilize this folder for your application.
    - If the disk is not moutned at all, we ask if you would like to install in ~/harmony as a work around for now but beware your storage space with this option!!!

