---
## >-
  Grant a group sudoless access and add the user or give the user root access
  directly.
---

# Sudoless Root Access

As your root account, use the editor of your choice modify the file `/etc/sudoers` as show \(nano example below\):

```text
sudo nano /etc/sudoers
```

Inside of the file add a new line with your user account name. We've added `serviceharmony` in our example below:

```text
serviceharmony ALL=(ALL) NOPASSWD:ALL
```

Save the file and exit.

You'll need to disconnect your account and reconnect before the permissions are enabled. After reconnecting you are ready to run the easy-node-installer Application or validator-toolbox Application.

