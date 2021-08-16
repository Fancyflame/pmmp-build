# pmmp-build
The PHP build script for PocketMine-MP on Android target with native compilation (Termux).

## Why it exist
To support server feature of MCMU on Android, PocketMine-MP is needed. But without other Linux device and official script didn't support Android native compilation, I modified official `compile.sh` to realize it.

## How to use
This shell should be run on **Android environment** like Termux. This shell **DO NOT** prevent you from running it on other platform, which may cause unexpected error!

```shell

# clone official git repository on your current directory
git clone https://github.com/pmmp/php-build-scripts.git
cd php-build-scripts

# clone this git repository
git clone https://github.com/Fancyflame/pmmp-build.git

# cover official's compile.sh
mv pmmp-build/compile.sh .
rm -r pmmp-build

# compile! (run with 8 threads to make)
./compile.sh -j8

# start!
./start.sh

```
