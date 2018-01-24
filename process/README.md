# Linux Process

How to get the directory from which the process has been started.

Each process will have a directory created in `/proc/<process_id>`, list the folders using `ls -ltr` and see `cwd` link, which is the actual directory where the process has been started.