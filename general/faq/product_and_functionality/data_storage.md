## How is sensitive user data stored?
Both on iOS and Android devices, user data is encrypted and stored locally, only the Termius app has access to this data. The encryption being used on Android is AES-256 and ‘[industry-standard encryption techniques](https://support.apple.com/en-us/HT202303)’ on iOS.

Now in case you have a premium account, user data will be synchronized with all your devices. To do so, we use our own Zero-knowledge data storage. Before synchronization, all data will be encrypted on the client side, using AES-256 and your personal master password. Only encrypted data is being synchronized with our Servers, and neither the SecretKey nor your master password is stored on our servers.

Our Chrome extension saves user data directly to our back-end. All data is encrypted using AES-256 in combination with your personal master password. Different to the devices, our Chrome extension allows you to save the master password, in case you wish to.

###### [[Go Back](README.md)]
