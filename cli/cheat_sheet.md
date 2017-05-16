# Cheat sheet
###### [[Termius Documentation](/README.md) > [CLI Tool](/README.md)]

This cheat sheet gives ready examples that helps you to get your job done using the CLI tool. Be aware that using the CLI tool requires some basic knowledge of working with the Command Line Interface.

### In this document
* [Import multiple hosts](#how-to-import-multiple-hosts)

## How to import multiple hosts?
Every now and then users ask us whether there's an easy way to add multiple hosts to Termius. To help out, we have written a simple script that does the trick (crudely, but it works).

### Requirements
- A MacOS, Linux or Windows PC
- Python and Termius CLI preinstalled
- The importer.py script
- A source.txt file with the hosts and details

> ###### *!* importer.py is capable of importing Hostname, Address, Username and Password only. You may need to modify the script to import other host details.

### First things first
Before you continue, run the commands that I've written below, using the terminal. If `Pull data from Termius cloud.` returns you may continue. Otherwise, you have encountered a bug which we will fix in a future release of the CLI tool.

```
Termius login
Termius pull
```

### Getting the source.txt file ready
The source file is a plain text file. Each new line is considered a new entry. Values are separated by a comma (,). The source file follows the following pattern and blank fields are ignored:
`{Name}.{Address},{Username},{Password}`

Your file could look like the following:

```
Router,192.168.1.1,admin,admin
Raspberry pi,192.168.1.15,pi,Raspberry
Home media center,192.168.1.16
Work,81.138.33.19
```

### Get importer.py

Download the importer.py script

{"gitdown": "gist", "id": "be08dd9864438a43bf25d8442d6c8437"}

<script src="https://gist.github.com/Dreamzilla/be08dd9864438a43bf25d8442d6c8437.js"></script>

> ***!*** Make sure importer.py and the source file are in the same directory!!

### Run importer.py

Now importer.py and source.txt are prepared you may run importer.py.
- Open the terminal
- Navigate to the directory that contains importer.py and source.txt
- Run `python importer.py source.txt`

The script will take a few seconds to initiate and you'll be prompted to login. You'll be asked to provide your password several times again. Note that processing may take a while, especially when you are importing a large amount of hosts.

> ***!*** It is wise to run a test on a smaller amount of hosts for verification
