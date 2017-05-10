# I’m getting a “handshake failed” error message, please help?
###### [[Termius Documentation](../../../README.md) > [General](../../README.md) > [FAQ](../README.md) > [Terminal and Troubleshooting](README.md)]

When a TCP connection is made by a client, the server responds with the protocol versions it supports, this process is called, the handshake. In case the server and client find a matching protocol, the handshake is successful, and the server and client will continue to negotiate the secure connection.

Otherwise, a failed handshake indicates that the server and client weren’t able to match protocols, and so a secure connection could not be established. The protocol version Termius supports are listed below.

If you get a `handshake failed` error message, it means that the server you’re trying to connect with is using an unsupported protocol version. In the future, we will add additional protocol versions. However, for now, the only work-around is a reconfiguration on the server side.

## Supported protocol versions
| iOS | Android | Chrome |
| ----- | ----- | ----- |
| __Key Exchange Methods:__ | __Key Exchange Methods:__ | __Key Exchange Methods:__ |
| Diffie-Hellman-group1-sha1 | Diffie-Hellman-group1-sha1 | Coming soon |
| Diffie-Hellman-group14-sha1 | Diffie-Hellman-group14-sha1 |  |
| Diffie-Hellman-group-exchange-sha1 | Diffie-Hellman-group-exchange-sha1 |  |
|  | Diffie-Hellman-group-exchange-sha256 |  |
|  | Ecdh-sha2-nistp256 |  |
|  | Ecdh-sha2-nistp384 |  |
|  | Ecdh-sha2-nistp521 |  |
| ----- | ----- | ----- |
| __Hostkey Types:__ | __Hostkey Types:__ |  |
| Ssh-rsa | Ssh-rsa |  |
| Ssh-dss | Ssh-dss |  |
| ----- | ----- | ------ |
| __Ciphers:__ | __Ciphers:__|  |
| AES256-cbc (rijndael-cbc@lysator.liu.se) | AES128-cbc |  |
| AES192-cbc | AES192-cbc |  |
| AES128-cbc | AES256-cbc |  |
| 3des-cbc | AES128-ctr |  |
| Blowfish-cbc | AES192-ctr |  |
| Cast128-cbc | AES256-ctr |  |
| Arcfour | 3des-cbc |  |
| none | 3des-ctr |  |
|  | Blowfish-cbc, |  |
|  | Arcfour |  |
|  | Arcfour128 |  |
|  | Arcfour256 |  |
|  | none |  |
| ----- | ----- | ----- |

###### [[Go Back](README.md)]
