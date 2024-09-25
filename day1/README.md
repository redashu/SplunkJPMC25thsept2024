## Splunk Basic 

<img src="spb1.png">

### more basic info 

<img src="spb2.png">

## basic Spluk Architecture level 1 

<img src="sparch.png">

### arch 2 

<img src="arch2.png">

### arch 22 

<img src="arch22.png">


### SPE setup 

<img src="setup1.png">

##  checking splunk LIcense and trails 

[click_here](https://www.splunk.com/en_us/download.html)


## Downloading SPlunk Enterpirse for linux 

```
wget -O splunk-9.3.1-0b8d769cb912.x86_64.rpm "https://download.splunk.com/products/splunk/releases/9.3.1/linux/splunk-9.3.1-0b8d769cb912.x86_64.rpm"
--2024-09-25 05:54:56--  https://download.splunk.com/products/splunk/releases/9.3.1/linux/splunk-9.3.1-0b8d769cb912.x86_64.rpm
Resolving download.splunk.com (download.splunk.com)... 3.167.37.9, 3.167.37.124, 3.167.37.110, ...
Connecting to download.splunk.com (download.splunk.com)|3.167.37.9|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 990009597 (944M) [binary/octet-stream]
Saving to: ‘splunk-9.3.1-0b8d769cb912.x86_64.rpm’

splunk-9.3.1-0b8d769cb912.x86_64.rpm   100%[=========================================================================>] 944.15M  76.6MB/s    in 12s     

2024-09-25 05:55:08 (76.6 MB/s) - ‘splunk-9.3.1-0b8d769cb912.x86_64.rpm’ saved [990009597/990009597]


===>>

[ec2-user@ip-172-31-80-225 ~]$ ls
splunk-9.3.1-0b8d769cb912.x86_64.rpm
[ec2-user@ip-172-31-80-225 ~]$ '

```

## Installing Splunk Enterprise license software on RHEL 

```
 sudo rpm -ivh splunk-9.3.1-0b8d769cb912.x86_64.rpm 
warning: splunk-9.3.1-0b8d769cb912.x86_64.rpm: Header V4 RSA/SHA256 Signature, key ID b3cd4420: NOKEY
Verifying...                          ################################# [100%]
Preparing...                          

===> Verify 

rpm -q splunk 
splunk-9.3.1-0b8d769cb912.x86_64
```