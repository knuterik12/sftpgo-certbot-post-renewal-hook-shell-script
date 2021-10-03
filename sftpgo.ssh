#!/bin/sh
sudo cp /etc/letsencrypt/live/server.com/fullchain.pem /etc/sftpgo/ssl/
sudo cp /etc/letsencrypt/live/server.com/privkey.pem /etc/sftpgo/ssl/
sudo chown -R sftpgo:sftpgo /etc/sftpgo/ssl
sudo systemctl reload sftpgo
