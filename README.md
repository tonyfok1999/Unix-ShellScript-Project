# Unix Recycle Bin Project
Since Unix file system doesn't have a recycle bin, whenever a file or directory is removed, it cannot be restored. The goal of this project is to create scripts to move files in and out of recycle bin, so that users can safely remove and restore files just like on the Windows or Mac OS.

## Recycle
### Description
This command recycles the specified file or folder (file inclusive) to $HOME/recyclebin

### Synopsis
```
bash recycle [OPTION]... [FILE]...
```

### Options
```
-i	Ask for confirmation before recycling any files. A response beginning with y or Y means yes. All other responses mean no.

-v	Display a message confirming recycle

-r	Remove a directory and recycle its contents
```

## Restore
### Description
This command restores individual files from $HOME/recyclebin back to their original location.  Recycled file path will be stored in ".restore.info"

### Synopsis
```
bash restore [OPTION] [FILE]...
```

```
-r	Restore files that were recycled from a directory previously
```
