# How to get the Termius CLI Tool
###### [[Termius Documentation](../README.md) > [CLI](README.md)]

The CLI tool is available for Linux, MacOS and Windows and can be installed using the following distribution channels:
- [Homebrew (MacOS)](#homebrew)
- [Curl (Linux)](#curl)
- [Pip (Python, Cross-Platform)](#pip)

After installation, check out our [Quick Start guide](quick_start/README.md) or [Cheat Sheet](cheat_sheet.md).

## Homebrew
For MacOS users, there is a [Homebrew](http://brew.sh/) formula available.
You may install the Termius CLI tool using your native terminal and the following command:

`$ brew install termius`

> ***!*** The command above installs Bash and zsh completions by default

## Curl
Linux users install a `bootstrap.sh` script. You use your native terminal and the following command:

`$ curl -sSL https://raw.githubusercontent.com/Crystalnix/termius-cli/master/bootstrap.sh | bash`

## Pip
If your platform does not support Homebrew or Curl, or if you prefer to use Python instead, we have made a Pip and Easy_install version available. Note that these versions **require Python to work** properly.

> ***!*** Make sure you have [Python installed](https://www.python.org/downloads/) with `pip` and `Add Python to environment variables` checked!

Prefer to use Pip? To install the Termius CLI tool, use your native terminal tool, or Windows PowerShell and the following command:

`pip install -U termius`

> ***!*** Prefer to use Eas_install instead? Try `easy_install -U termius`





###### [[Go Back](README.md)]
