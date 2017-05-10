## I've generated a key with a passphrase, but the passphrase is not requested on connecting
*Termius supports RSA, DSA, and ECDSA keys for passwordless login. And you may protect your private key using a passphrase. This means that the private key will be encrypted using a passphrase to add an extra layer of security.*

Passphrase-protected keys can be [generated](../../features/keychain.md#generate-a-key) by the key generator which you can find under `Keychain > Add > New key > Generate`. When you generate a passphrase-protected key set -- the public key, encrypted private key, **and passphrase** -- **will be stored in the Key chain**. Because of this, the passphrase will not be requested on the establishment of a connection. 

> ***!*** In the latest Termius (2.4.9), when you'll generate a new key, you'll find a checkbox `Save passphrase` that is checked by default. Uncheck this checkbox if you do not wish to store the passphrase.

In case you wish that the passphrase will be prompted, **just remove the passphrase** after key generation. To do so:
* Tap the particular key 
* A new screen `Edit Key` should pop up
* Tap the `Passphrase` field and remove its value
* And hit the tick `✓` in the top right corner

Now the passphrase will be prompted before a connection may be established.

![Remove the value of the passphrase field](../../.images/screenshots/passphrase-prompt.gif)


> ***!*** Note that you also may [import](../../features/keychain.md#import-keys) passphrase-protected keys. You only need to fill out the passphrase field if you wish to store the passphrase in Keychain
