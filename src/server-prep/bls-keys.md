# BLS Keys
Currently the toolbox doesn't assist with BLS Keys. Support is planned in a future release. Here's the notes from our original guide on BLS Keys.

## Setting up BLS Keys

### Our notes on BLS keys

We suggest making 10 BLS keys on the shard you start with. Save them to your home PC. They can be reused anytime you deploy that shard again and only need to be created once. Once you have your .key & .pass files save them in a folder at home for reuse via WinSCP, scp, rsync, or however you send files to a server.

When you start you won't need more than 1 for quite some time \(at least 9.5 million $ONE today\) but if you have the others in place you won't need to restart your services and miss blocks to add more keys to your nodes.

### Creating new BLS keys

This covers creation of your BLS Key\(s\) that you decided on before starting the guide. We encourage you to run one on shards 1-3 instead of just 0.

Here you'll be creating the keys, creating a folder, and copying them into the proper folders.

You may want to store a backup of these files as well.