
# TAR GZ
## for unzip
```
tar -xvzf build-marso-demo-shnaps.orig.tar.gz -C shnaps
```

- `f`: -- **F**ile. This must be the last flag of the command, and the tar **F**ile must be immediately after. It tells tar the name and path of the compressed file.
- `z`: -- g**Z**ip. Tells tar to decompress the archive using g**z**ip
- `x`: -- e**X**tract. Tar can collect files or e**x**tract them. `x` does the latter.
- `v`: -- **V**erbose. Makes tar talk a lot. **V**erbose output shows you all the files being extracted.
- `-t`, `--list`  List the contents of an archive. Arguments are optional. When given, they specify the names of the members to list.

## for ZIP
```
tar czf name_of_archive_file.tar.gz name_of_directory_to_tar
```

- `c` — create an archive file (as opposed to extract, which is `x`)
- `f` — filename of the archive file
- `z` — filter archive through `gzip` (remove this option to create a `.tar` file)

# ZIP

```
unzip file.zip -d destination_folder
```