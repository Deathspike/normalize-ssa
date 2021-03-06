# normalize-ssa

Extracts ssa/ass subtitle(s) from MKV videos and rescale/resize subtitles.

# Prerequisites

* NodeJS >= 14 (http://nodejs.org/)
* NPM >= 6 (https://www.npmjs.org/)

# Install

## Windows

1. Install *NodeJS* following the instructions at http://nodejs.org/
2. Run in *Command Prompt*: `npm install -g normalize-ssa`

## Mac OS X

1. Install *NodeJS* following the instructions at http://nodejs.org/
2. Run in *Terminal*: `npm install -g normalize-ssa`

## Debian (Mint, Ubuntu, etc)

1. Install *NodeJS* following the instructions at http://nodejs.org/
2. Run in *Terminal*: `sudo apt-get install ffmpeg`
3. Run in *Terminal*: `sudo npm install -g normalize-ssa`

# Update

## Windows

1. Ensure that `normalize-ssa` is [installed](#Install)
2. Run in *Command Prompt*: `npm install -g normalize-ssa`

## Mac OS X

1. Ensure that `normalize-ssa` is [installed](#Install)
2. Run in *Terminal*: `npm install -g normalize-ssa`

## Debian (Mint, Ubuntu, etc)

1. Ensure that `normalize-ssa` is [installed](#Install)
2. Run in *Terminal*: `sudo npm install -g normalize-ssa`

# Usage

```
Usage: normalize-ssa [options] [command]

Extracts ssa/ass subtitle(s) from MKV videos and rescale/resize subtitles.

Options:
  -V, --version                      output the version number
  -h, --help                         display help for command

Commands:
  parse [options] <resourcePath...>  Parse subtitle(s).
  help [command]                     display help for command
```

## Parse

To parse *subtitles* and rescale/resize, run:

    normalize-ssa parse /path/to/your/video.mkv

Or to recursively find and parse `.ass`/`.mkv` files in a directory, run:

    normalize-ssa parse /path/to/your/directory

To extract a different language than *English* from a `.mkv`, like `ger` for *German*, run:

    normalize-ssa parse -l ger /path/to/your/fileOrDirectory

And to select a different font size, run:

    normalize-ssa parse -s large /path/to/your/fileOrDirectory

The valid font sizes are `tiny`, `small`, `normal`, `large` or `huge`.

# Contributions

While software contributions are welcome, you can also help with:

* Documentation
* Helping other people
* Feature requests
* Bug reports

# Questions?

Please make an issue if you have questions, wish to request a feature, etc.
