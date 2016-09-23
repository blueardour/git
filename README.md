# git
git 1.8.5.3

The git software installed by apt does not include ssl functions. So I often compile it from source with libcurl4-openssl-dev.
Then issues like `server certificate verification failed. CAfile: /etc/ssl/certs/ca-certificates.crt CRLfile: none` could be solved.

Shy~~

TO do:
```
sudo apt-get install libcurl4-openssl-dev zip  
wget --no-check-certificate https://codeload.github.com/blueardour/git/zip/master
unzip master
cd git-master
tar xvf git-1.8.5.3.tar.gz
cd git-1.8.5.3
./configure && make && sudo make install
```

