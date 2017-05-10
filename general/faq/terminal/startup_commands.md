# I’ve noticed that Termius issues a couple of shell commands before starting the session. Why?
###### [[Termius Documentation](../../../README.md) > [General](../../README.md) > [FAQ](../README.md) > [Terminal and Troubleshooting](README.md)]

On opening a new connection Termius issues the following shell commands.

`````
HISTFILE=;SA_OS_TYPE="Linux"
REAL_OS_NAME=`uname`
if [ "$REAL_OS_NAME" != "$SA_OS_TYPE" ] ;
then
echo `uname`\nelse\nDISTRIB_ID=\\"`cat /etc/*release`\\"
echo $DISTRIB_ID;
fi;
exit;
`````

These commands detect the version of the OS you’re connecting to. They are executed automatically to render the appropriate icons, such as the Ubuntu, CentOS or FreeBSD logo, in the server listing.

This functionality can be disabled by toggling `Detect OS` `off` under settings.

###### [[Go Back](README.md)]
