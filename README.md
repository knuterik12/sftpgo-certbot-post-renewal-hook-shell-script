# sftpgo-certbot-post-renewal-hook-shell-script
How to install Certbot SSL/TLS certificates with auto renewal on the SFTPGO web UI

https://www.knuterikevensen.com/?p=11520

A certbot post renewal hook shell script to automatically copy the certificates to the sftgp ssl directory 
and change the ownership of the certificates to the sftpgo user and 
reload SFTPGO with SIGHUP, SFTPGO will reload the certifcates while not interrupting download and uploads.

Instructions 

place in

/etc/letsencrypt/renewal-hooks/post/sftpgo.sh

make the script executable

sudo chmod 755 /etc/letsencrypt/renewal-hooks/post/sftpgo.sh