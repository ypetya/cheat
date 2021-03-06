--- 
openssl: |-
  View a certificate:
    openssl x509 -in mycert.crt -text
  
  Remove passphrase from a key:
    openssl rsa -in server.key -out server-without-passphrase.key
  
  Generate a self-signed cert/key:
    openssl req -new -newkey rsa:2048 -days 365 -nodes -x509 -keyout server.key -out server.pem
  
  Encrypt and decrypt a single file:
    openssl aes-128-cbc -salt -in file -out file.aes
    openssl aes-128-cbc -d -salt -in file.aes -out file
  
  tar and encrypt a whole directory:
    tar -cf - directory | openssl aes-128-cbc -salt -out directory.tar.aes
    openssl aes-128-cbc -d -salt -in directory.tar.aes | tar -x
  
  tar zip and encrypt a whole directory:
    tar -zcf - directory | openssl aes-128-cbc -salt -out directory.tgz.aes
    openssl aes-128-cbc -d -salt -in directory.tgz.aes | tar -xz
  
  convert a .crt to .pem
    openssl x509 -inform DER -in ca_cert.crt -out ca_cert.pem -outform PEM
  
  print cert info
    openssl x509 -in ca_cert.pem -text -noout
  
  add CA cert to "trusted" (your unix distribution might have a different path to configuration). this will add a sym link with the hash as name
    cd /System/Library/OpenSSL/certs
    sudo ln -s ca_cert.pem `openssl x509 -hash -noout -in ca_cert.pem`.0
  
  verify a server cert against a CA
    openssl verify -CApath /System/Library/OpenSSL/certs/ /tmp/securesite.com.pem
  
  connect to a server (CApath to your distro)
    openssl s_client -CApath /System/Library/OpenSSL/certs/certs/ -connect securesite.com:443
  
  verify private key match
    openssl x509 -noout -modulus -in server.pem | openssl md5 ;\
    openssl rsa -noout -modulus -in server.key | openssl md5
