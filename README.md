# nmap-sublime-syntax
Project that aims to provide syntax highlighting to NMAP reports when opened with [bat](https://github.com/sharkdp/bat) or with [Sublime Text](https://www.sublimetext.com/).

## Installation
- Clone this repo: `https://github.com/ToniIvars/nmap-sublime-syntax && cd nmap-sublime-syntax`
- Create a folder with syntax definition files: `mkdir -p "$(bat --config-dir)/syntaxes"`
- Copy the syntax file to the folder you have just created: `cp nmap.sublime-syntax "$(bat --config-dir)/syntaxes"`
- Make the NMAP syntax available: `bat cache --build`
- OPTIONAL: Remove the repo: `cd ../ && rm -rf nmap-sublime-syntax`

## Usage
With **bat**, you can use this syntax extension in two different ways:
1. Save the file with **.nmap** extension. When you run the bat command, it will load the appropiate syntax automatically.
2. Run bat with the **-l nmap** flag.