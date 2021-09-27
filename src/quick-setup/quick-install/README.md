---
description: Here's the short guide on installing and our notes.
---

# Quick Install

## New Validators

This guide won't work out so well for absolutely new users. You should go through the [New Validator Steps](../../full-manual/pre-installation-information/new-validator-steps/) and setup a node that way before you attempt the quick version.

## Server Prep:

* ✔️ A new Ubuntu 20.04LTS server
* ✔️ Login as a user account with sudoless root access or run and install as root
  * Digital Ocean Admins: Use the [same guide](../../full-manual/server-prep/digital-ocean.md) as our validator-toolbox Application to setup "User Data" on your Digital Ocean Droplet.
  * Other Providers Admins: Use the [Any Other Provider Guide](../../full-manual/server-prep/any-other-provider/) on how to edit your [sudoers file](../../full-manual/server-prep/any-other-provider/sudoless-root-access.md) or give access via groups.
* ✔️ Volume Support
  * Digital Ocean Auto Mounted Volumes will be detected and used for installation
  * Other Providers: Mount your volume in /mnt and it will be detected and used for installation

That's it for the requirements, you're ready to connect to your new server and install the Harmony Validator Server Node software.

## Pull & Install on a New or Existing Server:

Pull the repository into your home directory.

```bash
cd ~/
git clone https://github.com/easy-node-one/validatortoolbox.git
```

Install requirements.

```bash
cd validatortoolbox
sudo apt-get install dnsutils python3-pip python3-dotenv -y
pip3 install -r requirements.txt
```

Run the installer from anywhere.

```text
python3 ~/validatortoolbox/toolbox/start.py
```

## First load of application on any server/system:

The first time you run the python application we will build environment settings in ~/.easynode.env

You will be presented with menus to choose your preferred node setup:

![Run the Server Node Installer \(New Servers\) or just run the Validator Toolbox Menu \(Existing\)](../../.gitbook/assets/image%20%2825%29.png)

Continue onto our [Setup Menus](../../full-manual/installation/setup-menus.md) section of the main guide for more information on each available choice during our guided menu installer.
