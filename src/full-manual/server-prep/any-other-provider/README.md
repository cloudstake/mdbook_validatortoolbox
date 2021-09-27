# Any Other Provider
---
#### Here's what you need to get done to install validator-toolbox on a brand new Ubuntu 20.04LTS Server that you plan to run as a Harmony ONE Validator.
## Server providers not named Digital Ocean:

Here's what **you need to setup** for our application to run smoothly the first time you want to setup a new node:

* **Operating System**
  * Ubuntu 20.04LTS - The suggested operating system from harmony
* **Account**
  * Be logged into any user account, **we strongly suggest not using root**.
  * Account must have [sudoless root access](sudoless-root-access.md) \(if not using the root account\)
  * If you skip this step, you will be prompted for your password during rclone setup but it will be hidden in the menu. If it pauses there type your user account password.
* **Storage Volume**
  * Mount your volume to any folder inside of /mnt and we'll detect a single mount point inside of that folder, install harmony in /mnt/yourfolder/harmony and symlink that folder to ~/harmony

