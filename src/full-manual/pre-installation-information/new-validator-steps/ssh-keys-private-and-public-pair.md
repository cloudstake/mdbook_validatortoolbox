---
description: >-
  How to further secure your server with passwordless login via ssh
  private/public keys for your VPS provider & Github
---

# SSH Keys - Private & Public Pair

If you're using a cloud service for a provider you are most always prompted to upload your public key for the service provider to install on your new server \(or droplet if it's [Digital Ocean](https://m.do.co/c/b761e5fdd694)\).

Disabling password logins on your server and only using SSH keys is a great way to harden the security of your node. With proper firewall configuration and SSH keys you can seriously lock down the security and make it virtually impossible for attackers to get into your node.

Here's the guide on creating private & public key pairs to use:

## Create your key pairs

We suggest running the following command in linux or windows 10 powershell to generate an ssh public & private key pair on your system. After running the command you will be asked a series of questions. If this is your first time running the command it's ok to just hit enter and use defaults for all of these. If you would like to add a password to your key you can but it's not required and will prompt you every time you use it if a password is applied.

`ssh-keygen -t rsa -b 4096`

![](../../../.gitbook/assets/image%20%286%29.png)

This will create the files id\_rsa & id\_rsa.pub in your user's home directory in the ~/.ssh folder. On windows it goes into C:\users\\[your\_username\].ssh folder.

If you head over to your provider's website, you will be able to upload the contents of your id\_rsa.pub folder into the security section of your account. Find the area to add an SSH key, give it a label \(usually the PC you made the key on so you know where it lives\) and paste the entire contents of your id\_rsa.pub file into the box. Press save and you'll now have the key ready to load when creating a new server on that service provider.

This is also a great time to create a github account and upload your public key to the settings section of that account as well. As a validator operator you'll find yourself using github often and ssh access is the best. It also sets up your public key for anyone to use to give you access to servers. You can find your key by modifying the username at the end of this url, here's ours for example: [https://github.com/patrickmogul.keys](https://github.com/patrickmogul.keys)

