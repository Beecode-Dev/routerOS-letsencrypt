# routerOS-letsencrypt
Lets Encrypt renewal with automatic assignment of the certificate to active hotspots SSL

1. Create a Script named "LetsEncrypt-Renewal" (System -> Scripts) with read and write permissions.
2. modify the variable dnsName with your own.
3. paste the script.txt into the script field.
4. Create a Scheduler
   `/system scheduler add interval=1d name=LetsEncrypt-Renewal on-event=LetsEncrypt-Renewal policy=read,write start-time=03:00:00`
