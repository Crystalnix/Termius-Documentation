# Is my data secure with Termius?
###### [[Termius Documentation](../README.md) > [General](README.md)]

Termius handles sensitive data with the greatest care. On all our supported platforms, user data is encrypted and stored locally, only the Termius app has access to this data. The encryption being used on Android is AES-256 and ‘industry-standard encryption techniques’ on iOS.

Now in case you have a premium account, user data will be synchronized with all your devices. To do so, we use our own Zero-knowledge data storage. Before synchronization, all data will be encrypted on the client side, using AES-256 and your personal master password. Only encrypted data is being synchronized with our Servers, and neither the SecretKey nor your master password is stored on our servers.

To add an extra layer of security, you may [enable 2 Factor Authentication](what_is_2fa.md).

###### [[Go Back](README.md)]
