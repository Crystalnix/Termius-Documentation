## Is it possible to disable synchronization?

Synchronization is not disableable, but you can disable the synchronization of SSH password and key synchronization. To do so, **Android** users navigate to `Settings > Security`, and toggle `Sync keys and identities` off. **iOS** users navigate to `Settings > Synchronization` and uncheck `Keys & Passwords Sync`.

> **!** We use AWS as storage and all data is stored according to the zero-knowledge principle. All information is encrypted on the client side before synchronization. The encryption key and hash are never stored remotely, so only you will be able to access your data.

[[Go Back](README.md)]
