## ```ls``` command
- shows version : ls --version
- show help page : ls --help
- list files and directories in bare format : ls
- file or directory, size, modified date and time, file or folder name and owner of file and its permission : ls -l
- list all files including hidden file starting with ‘.‘. : ls -la
- list files with human readable format : ls -lh
- list file size for all of them but without any other additional details : ls -sh
- list files and directories with ‘/’ character at the end : ls -F
- prints out directories and files separated by a comma : ls -m
- add quotation marks to all directories and files : ls -Q
- list files in reverse order : ls -r
- recursively list sub-directories : ls -R
- display UID and GID of files and directories: ls -n
- display inode number (unique number in linux) of file or directory : ls -i
- sort files by time and date modified : ls -t
- sort files by file extension type: ls -X
- sort files by file size (displays file size in order, will display big in size first) : ls -lS
- reverse output order will shows latest modification file or directory date as last : ls -ltr
- list directory information (list files under directory) : ls -l /tmp
- list directory information (displays information of directory) : ls -ld /tmp


tips:
- alias ls="ls -lahF --color=auto"
