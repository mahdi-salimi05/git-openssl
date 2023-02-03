# git-openssl
a git Package with openssl
```
source: https://stackoverflow.com/questions/51088635/git-clone-error-gnutls-handshake-failed-an-unexpected-tls-packet-was-receive
```
fatal: unable to access '<my_git>.git/': gnutls_handshake() failed: An unexpected TLS packet was received.
 
 Might be issue with gnutls Package. we have to install a git Package with openssl instead of gnutls. Follow the below steps,
```
sudo apt-get install -y libcurl4-openssl-dev
sudo dpkg -i <git-openssl from release page>
 
```
