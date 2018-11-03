1. Get current disk usage

   df -h
   
2. Get current directory usage

   du -h
   
3. Get disk usage by directory by directory

   du -h --max-depth=1 . | sort -n

4. Formatting a disk (Ex: for newly attached AWS EBS to EC2 instance)

Good documentation available on 

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-using-volumes.html


Giving read, write and execute permissions on the folder

chmod 777 -R /data

