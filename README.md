# rclone-edit

Edit files in cloud storage with $EDITOR.

`rclone-edit rcloneremote:test.txt` will open test.txt from rcloneremote in `nano` (or `$EDITOR`), and save changes back to rcloneremote on exit.

Basically just `rclone cat $1 | vipe | rclone rcat $1`, but using bundled vipe if [moreutils](https://joeyh.name/code/moreutils/) not installed and defaulting to nano.

## Installation

Copy/symlink `rclone-edit` to a location in `$PATH`, like `/usr/local/bin` and make sure that it is executable with `chmod +x <path to rclone-edit`>
