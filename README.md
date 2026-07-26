# Gaztag (a tagger for Gazelle trackers)
Supports RED and OPS, just dump your fresh downloads into a folder (I use a ramdisk) and run `$ gaztag run` and watch it go.

Tags album versions, genres, downloads album art, sorts scans and booklets, flattens multi-disk albums, renames files and directories... and such.

Edit the config file and put it in ~/.config/gaztag/config.toml

![demo gif](https://github.com/benjamindaines/gaztag/blob/master/demo.gif?raw=true)
(I promise I don't use nano... don't judge. Would be hilarious, but rude to hard-code vim as the editor 😁)
![screenshot](https://github.com/benjamindaines/gaztag/blob/master/screenshot.png?raw=true)

```
usage: gaztag [-h] [--config CONFIG] [--plan PLAN] [--dest DEST] [--dry-run] [--force-art] [-q]
              {run,plan,apply,auth} ...

gaztag: source album metadata from a Gazelle tracker and organize local music.

positional arguments:
  {run,plan,apply,auth}
    run                 plan, confirm, then apply
    plan                resolve metadata and write a plan
    apply               execute a previously written plan
    auth                validate the API key and print the account identity

options:
  -h, --help            show this help message and exit
  --config CONFIG
  --plan PLAN
  --dest DEST           destination root override
  --dry-run
  --force-art
  -q, --quiet           suppress progress output
```
