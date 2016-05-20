1. Get current disk usage

   df -h
   
2. Get current directory usage

   du -h
   
3. Get disk usage by directory by directory

   du -h --max-depth=1 . | sort -n