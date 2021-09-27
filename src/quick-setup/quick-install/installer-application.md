---
## Installing Harmony Validator software on a new Signing or Non-Signing Node
---

# Installer Application

## Installer Choices

![Just our loading screen, first time you run it, the bottom banner will read this.](../../.gitbook/assets/image%20%2835%29.png)

## Shard Choice

Pick the shard you want the server you're running your software on to use.

![Choose the shard for your node](../../.gitbook/assets/image%20%2827%29.png)

## Standard Signing Node or Full Non-Signing Validator

* Standard Signing Node - Regular Harmony Validators are Standard Signing Nodes
* Full Nodes Dev/RPC - Non-signing nodes used for development and RPC services

![Choose your node type, Signing or Non-Siging](../../.gitbook/assets/image%20%2826%29.png)

## Mainnet or Testnet

Mainnet or Testnet? We support both!

![Choose the network you will run on.](../../.gitbook/assets/image%20%2824%29.png)

## Express or Manual Install

Express will assume all options for the type you chose earlier \(Standard Signing or Full Non-Signing\). Manual Install will let you select y/n on every option along the way for max control. Most users will want to do the express installation.

![Express or manual](../../.gitbook/assets/image%20%2831%29.png)

## Signing Nodes Only - Wallet Recovery

Signing nodes will have the wallet password captured to ~/harmony/passphrase.txt where it would also be utilized by autobidder.

![Passing password through to file for future usage](../../.gitbook/assets/image%20%2832%29.png)

After setting up your wallet password, you will be prompted to directly input your mnemonic phrase into the hmy application via it's interface. We do not store or save your mnemonic data. You can hit ctrl+c to skip this and setup your wallet manually after installation.

![Waiting for mnemonic phrase to recover your validator wallet](../../.gitbook/assets/image%20%2828%29.png)

![Successful recovery of your wallet with address verification](../../.gitbook/assets/image%20%2830%29.png)

## Now Cloning Shards

We will now download your shards in reverse order if you're on shards 1-3. You can cancel shard downloads at anytime by pressing ctrl+c and manually complete them later.

Once we're at this point, you can connect another terminal and load your BLS keys or create new ones for this server.

![](../../.gitbook/assets/image%20%2829%29.png)

## Install Completed

The installer has finished running.

You will need to complete the following before your validator is operational:

* Place a BLS key \(or more\) into ~/harmony/.hmy/blskeys/
* Reboot your server

After a reboot, the node will automatically begin syncing with the blockchain if your keys are properly stored.

## Run Menu Application

You can relaunch our start.py script with the same command to load the menu application.

