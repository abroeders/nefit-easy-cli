# Nefit Easy™ command line interface

Command line interface for communications with Nefit/Bosch backend.

## Installation

```
$ npm i robertklep/nefit-easy-cli -g
```

This will install the `easy` client in a well-known "bin/" directory (`npm
config get prefix` will show you where)

## Options

```
$ easy -h

easy – Nefit Easy™ client

Usage:
  easy [options] status
  easy [options] pressure
  easy [options] location
  easy [options] active-program
  easy [options] program-data
  easy [options] display-code
  easy [options] get <uri>
  easy [options] put <uri> <data>
  easy [options] set temperature <value>
  easy [options] set active-program <value>
  easy [options] decrypt [--type=<type>] <base64>

Options:
  -h --help                   Show this screen
  -v --version                Show version
  -V --verbose                Be more verbose
  --pretty                    Pretty-print JSON output
  -s --serial=SERIAL          Nefit Easy™ serial number
  -a --access-key=ACCESS_KEY  Nefit Easy™ access key
  -p --password=PASSWORD      Nefit Easy™ password
  --type=<type>               Message type ('chat', 'alarm', 'email') [default: chat]

Instead of specifying serial number, access key or password through
options, you can also define them through environment variables:

  NEFIT_SERIAL_NUMBER
  NEFIT_ACCESS_KEY
  NEFIT_PASSWORD
```