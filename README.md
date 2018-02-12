# ssci
Install self signed certificate for a domain in cPanel.

### Usage
```
Usage: ssci [domain]
Example: ssci example.com
```

### Prerequisites
**jq** is needed for json parsing. cPanel api gives out the result in json, which is why it is needed. You can install it simply by typying the below in to the terminal:
```
yum install jq
```

### Installing
```
mkdir ~/bin
cd ~/bin
echo export PATH=\$PATH:$PWD >> ~/.bashrc
source ~/.bashrc
cd ~
git clone https://github.com/nake89/ssci
mv ssci/ .ssci
cd .ssci
chmod u+x ssci
ln -s ~/.ssci/ssci ~/bin/ssci
```
