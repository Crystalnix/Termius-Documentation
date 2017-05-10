## Connect to a host

After you’ve saved the new host, you’ll be sent back to the `Hosts` screen. Otherwise, make sure you're in the `Hosts` screen. Here you’ll find the new entry.

Tap the host you'd like to connect to once, when the connection works you’ll see a [security warning](http://www.lysium.de/blog/index.php?/archives/186-How-to-get-ssh-server-fingerprint-information.html). Don’t worry, everything is fine, click ‘Continue’. You’ll only see this warning the first time Termius connects to a Pi that it hasn’t seen before.

![Termius ‘Security warning’](../../.images/screenshots/ssh-ios-warning.png)

Now a terminal with a prompt should appear, you are connected. Type exit to close the terminal window.

![Termius Terminal](../../.images/screenshots/ssh-ios-window.png)

> **!** You can type `exit` to close the terminal window.

<br>

> ###Troubleshooting
> In case a red exclamation mark will appear, something went wrong. Tap the exclamation mark for the error description. ‘Connection establishment time out.’  means you’ve most likely entered a wrong IP address. Otherwise, you device might not be hooked up to a network, the host might be turned off, or it may be in a different network than your device.
