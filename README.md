# sftpgo-certbot-post-renewal-hook-shell-script
Activate SSL/TLS on the SFTPGO web UI with CERTBOT and auto renewal of the certificates

https://www.knuterikevensen.com/?p=11624

A certbot post renewal hook shell script to automatically copy the certificates to the sftgp ssl directory 
and change the ownership of the certificates to the sftpgo user and 
reload SFTPGO with SIGHUP, SFTPGO will reload the certifcates while not interrupting download and uploads.

Instructions 

place in

/etc/letsencrypt/renewal-hooks/post/sftpgo.sh

make the script executable

sudo chmod 755 /etc/letsencrypt/renewal-hooks/post/sftpgo.sh
