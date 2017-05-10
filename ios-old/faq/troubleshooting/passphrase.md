## I've generated a key with a passphrase, but the passphrase is not requested on connecting

*Termius supports RSA, DSA, and ECDSA keys for passwordless login. And you may protect your private key using a passphrase. This means that the private key will be encrypted using a passphrase to add an additional layer of security.*

Passphrase-protected keys can be [generated](#)[link missing] by the key generator which you can find under `Keychain > Add > New key > Generate`. When you generate a passphrase-protected key set -- the public key, encrypted private key, **and passphrase** -- **will be stored in the Key chain**. Because of this, the passphrase will not be requested on the establishment of a connection. 

In case you wish that the passphrase will be prompted, **simply remove the passphrase** after key generation. To do so:
* Slide the specific key to the left
* The `Export`, `Edit` and `Delete` options will now appear 
* Hit `Edit`, a new screen should pop up
* Tap and hold the `Passphrase` field and remove its value
* And hit `Save` in the top right corner

Now the passphrase will be prompted before a connection may be established.

![Remove the value of the passphrase field](../../.images/screenshots/passphrase-prompt.gif)

> ***!*** Note that you also may [import](https://github.com/Crystalnix/Termius-Documentation/blob/1e5521eb9e93e2fdbdf22378ddbe3424e9340c7e/android/features/keychain.md#import-keys) passphrase-protected keys. You only need to fill out the passphrase field if you wish to store the passphrase in Keychain
