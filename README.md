# 🎒 inventory
>
> Count files, view file size

## Installation

```sh
git clone https://github.com/teccdev/inventory.git
cd inventory
chmod +x inventory
mv inventory ~/.local/bin  # (or wherever you keep your scripts) 
```

If inventory doesn't work after installation, make sure the directory you moved it to is in your PATH

## Cleanup

(optional) You can remove the git repo afterward if you've moved the script:

```sh
cd ..
rm -rf inventory
```

## Usage

You can access this help at any time with `inventory --help`

```txt
Usage: inventory <mode> [options] [target]
Modes:
  -c, --count       Count files in the target directory
  -s, --size        Show size of the target file or directory

Options:
  -h, --help        Show this help message
  -r, --recursive   Process directories recursively (for count mode)
  -N, --N-decimals  Number of decimal places to show (e.g., -2 for 2 decimal places)
  -KB, --kilobytes  Show size in kilobytes (for size mode)
  -MB, --megabytes  Show size in megabytes (for size mode)
  -GB, --gigabytes  Show size in gigabytes (for size mode)

Examples:
  inventory -c /path/to/dir     Count files in directory
  inventory -s -r /path/to/dir  Show recursive size of directory
  inventory -s -2 file.txt      Show file size with 2 decimal places
  inventory -s -MB file.txt     Show file size in megabytes
```
