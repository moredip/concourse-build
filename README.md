# How do I make it go?
```
vagrant up
open http://192.168.100.27:8080/
```

## setting up the fly cli
We manage concourse pipelines using the `fly` cli tool. You can download it from your concourse instance. These links should work for you if you used `vagrant up`: [mac](http://192.168.100.27:8080/api/v1/cli?arch=amd64&platform=darwin) [linux](http://192.168.100.27:8080/api/v1/cli?arch=amd64&platform=linux) [windows](http://192.168.100.27:8080/api/v1/cli?arch=amd64&platform=windows). 

For convenience, place the fly cli tool somewhere in your $PATH. Here's one approach:
```
mkdir -p ~/bin
export $PATH=$PATH:~/bin
curl -o ~/bin/fly "http://192.168.100.27:8080/api/v1/cli?arch=amd64&platform=darwin"
chmod u+x ~/bin/fly
```

