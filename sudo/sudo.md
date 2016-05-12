1. Avoid prompt password for sudo
  
   echo 'password' | sudo -S command
  
   or 
  
   sudo visudo
  
   username ALL = NOPASSWD : ALL