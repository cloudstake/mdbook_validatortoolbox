# How to stop worrying and pick a shard
---
As of 9/24/21 most transactions happen on Shard 0 and it has the largest database size. Every server node deployed always has to have Shard 0, along with the database for Shards 1-3 if you're operating on one of those shards.

We encourage single key/slot validators to stay off of shard 0 at the current time as the hardware costs are 2x the cost on shards 1-3 and there's also a higher risk of having data overage costs on shard 0 as we saw in June during the spam attack on validators.

We suggest looking at the smart stake site and determining which shard of 1-3 has the lowest \# of keys and using that shard (https://harmony.smartstake.io/election - look at the top to compare numbers for shards 0-3).

If you grow large enough and want to contribute on Shard 0 later you can simply change keys at an epoch election to switch to new servers on a new shard \#.

