# Simple-FTP-server
A simple version of FTP server written in C


How to install:

cd to the ftp dir
make run [localhost] [port number()]
execute with ./ftp
Commands that are currently implemented:

USER PASS - cs317 ftp only at the moment, no password needed.
PASV NLST RETR QUIT TYPE 


Server currently works with linux only because of splice() and sendfile() functions. It should be easy enough
to implement RETR for other systems too.

This server currently doesn't support ASCII mode but this sould not be a problem with any modern system or ftp client.
