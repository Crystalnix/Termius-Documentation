## I've generated a key with a passphrase, but the passphrase is not requested on connecting

Termius supports RSA, DSA, and ECDSA keys for passwordless login. And you may protect your private key using a passphrase. This means that the private key will be encrypted using a passphrase to add an extra layer of security. Termius **stores the passphrase** together with the key's other values in the keychain. Because of this, the passphrase will not be requested on the establishment of a connection.

In case you wish that the passphrase will be prompted, **just remove the passphrase** from the key's settings in the Keychain.
* Navigate to the specific key
* Remove the value if the `Passphrase` field

For detailed instructions [Android users click here](../../../android/faq/troubleshooting/passphrase.md) and [iOS users click here](../../../ios/faq/troubleshooting/passphrase.md).

###### [[Go Back](README.md)]
