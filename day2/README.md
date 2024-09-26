## Revision 

<img src="rev1.png">

### Rev2 

<img src="rev2.png">

## Splunk forwarder commands 

```
===> status  check 

sudo /opt/splunkforwarder/bin/splunk status

===> Enterprise server list detail 

sudo /opt/splunkforwarder/bin/splunk   list forward-server

====> list monitor 

 sudo /opt/splunkforwarder/bin/splunk   list  monitor 
```

### starting httpd app to access app 

```
sudo systemctl start httpd
```

### Understanding Splunk Enterprise server -- Indexer 

<img src="indexer1.png">

### How to Interact with search head using SPL 

<img src="spl4.png">

# SPL 

### Example 1 

```
index="main" host="ip-172-31-80-225.ec2.internal"  ( sourcetype="access_log-too_small" OR sourcetype="access_combined" )
```

### Example 2 

```
index="main"  ( sourcetype="access_log-too_small" OR sourcetype="access_combined" ) | stats count by host | where count > 300 | sort count

```

### Example 3 

```
index="main"  ( sourcetype="access_log-too_small" OR sourcetype="access_combined" ) host="ip-172-31-80-225.ec2.internal" status>=400 status<500 |  stats count by clientip | where count > 2 | sort - count

```

### Example 4 

