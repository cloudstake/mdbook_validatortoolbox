---
description: >-
  Here's what you need to get done before you start setting up server equipment
  or virtual private servers.
---

# New Validator Steps

There's a lot of stuff to cover before you even create a node. 

Be sure to review our [Validator Operator Companion Guide](https://guides.easynode.one) before jumping in as it'll provide a deep overview of all the things you should know deeper about your server & software. 

_**However**_ you no longer need to know **all** of the guide as our installer will guide you through setup of a Harmony Validator Node. This reduces the learning curve greatly for simply setting up your server which is only one small hurdle on the path to becoming a validator.

With this in mind, here's a few concepts you need to be extra familiar with and do more research on:

* **BLS Keys**
  * How to [create BLS Keys & Pass Files](https://docs.harmony.one/home/network/validators/node-setup/generating-a-bls-key).
  * Where to store BLS Keys \(If you use our installer, they live in **~/harmony/.hmy/blskeys/**\)
  * How to Backup to your home machine or cloud for recovery
    * We suggest learning how to use `scp` or `rsync` or a [graphical application](https://companion.easynode.one/before-node-setup/admin-tools) to transfer files.

## TL;DR

Here's the TL;DR of what we cover on the next few pages of this section but that won't help you get a node running. You'll have to go through each of these on your path to becoming a validator.

* Sign up on [Digital Ocean](https://m.do.co/c/b761e5fdd694) and rent server, or utilize another provider of your choice
* Determine shard choice. Personal Preference but we strongly encourage _**NOT Shard 0**_ for many reasons for new validators.
  * \(1-3 recommended at this time for single key validators\)
* Create ssh key pub/priv pairs for use to auth on cloud provider service
* Create a github account and upload your .pub key to it so you can see it @ github.com/username.keys
* Create a brand for your validator
* Create a keybase account with your validator logo
* Setup SSH tools for your workstation \(Will you be using Windows or MAC to connect to your Ubuntu Linux Server?\) - Mobaxterm is our windows recommendation

