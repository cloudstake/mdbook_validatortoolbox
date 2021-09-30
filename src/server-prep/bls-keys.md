# BLS Keys
Currently the toolbox doesn't assist with BLS Keys. Support is planned in a future release. Here's the notes from our original guide on BLS Keys.

## Setting up BLS Keys

We suggest making 10 BLS keys on the shard you start with. Save them to your home PC. They can be reused anytime you deploy that shard again and only need to be created once. Once you have your .key & .pass files save them in a folder at home for reuse via WinSCP, scp, rsync, or however you send files to a server.

When you start you won't need more than 1 for quite some time \(at least 9.5 million $ONE today\) but if you have the others in place you won't need to restart your services and miss blocks to add more keys to your nodes.

### Creating new BLS keys

This covers creation of your BLS Key\(s\) that you decided on before starting the guide. We encourage you to run one on shards 1-3 instead of just 0.

Here you'll be creating the keys, creating a folder, and copying them into the proper folders. You may want to store a backup of these files as well.

To keep things simple, set up a password file before you begin. This will make it easy to copy the password to the required .pass files.

```s
echo -E 'password' > blskey.pass
```

To create BLS Keys after you've completed the toolbox installation:

```s
cd ~/harmony
./hmy keys generate-bls-keys --count 10 --shard 1 --passphrase-file blskey.pass
```

This will create .key files in your ~/harmony directory. Copy those key files to your ~/harmony/.hmy/blskey folder.
```s
cp *.key ~/harmony/.hmy/blskeys
```

The last step to use your blskey.pass file is to edit your harmony.conf file and setup the path.

```s
nano ~/harmony/harmony.conf
```

Change the line `PassFile = []` to read:
```s
PassFile = "./blskey.pass"
```

Save and exit nano (Ctrl+X y enter)

## Backup your .key and .pass files @ home or in the cloud

Using your [admin transfer tool](../pre-installation/new-validator-steps/system-administrator-tools.html) of choice, transfer your .key and .pass files to your home pc and store them securely. The key and pass files are all you need backed up to quickly restore a node. Once you create keys for a shard you can save them and re-use them when needed. They do not need to be created again once you have working copies backed up.

We suggest building a folder that contains a folder for each shard and storing your keys in there.