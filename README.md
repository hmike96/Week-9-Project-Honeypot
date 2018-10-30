# Week-9-Project-Honeypot

## Which Honeypot(s) you deployed
I deployed the Dionaea and the Snort honeypots to my MHN server.

## Any issues you encountered
I had most of my issues getting mhn set up. The first issue I had was around the repo we were told to download. It included a repo when installed that no longer existed so I had to switch to the repo https://github.com/threatstream/mhn#honeypot. After i did this the download took a lot longer but I ended up getting it to run. The next problem I had happened when I attempted to log in to nhm. It was not recognizing my password and username so I had to reset it using these instructions https://github.com/threatstream/MHN/wiki/MHN-Troubleshooting-Guide#i-have-an-internally-deployed-honeypot-and-even-when-i-scan-it-i-see-not-events-in-mhn. After I reset it, it allowed me to log in. After setting up the honeypot I was getting no attack data from it so after looking around for awhile I then had to use this solution to start getting attack data https://github.com/threatstream/MHN/wiki/MHN-Troubleshooting-Guide#i-have-an-internally-deployed-honeypot-and-even-when-i-scan-it-i-see-not-events-in-mhn. After I got past these road blocks I was able to start getting attack data for my honeypots. I also had an issue setting up the elastichoney honeypot so I used snort instead. To set up elastichoney I believe you have to update the node its on before using wgets.

## A summary of the data collected: number of attacks, number of malware samples, etc.
The features in the data include its id, oid, protocol, hpfeed_id, time, date, source_ip, source_port, destination_port, identifier, honeypot. And example data point is this.
{ "_id" : { "$oid" : "5bd7abfa616a1e2e0d40bb50" }, "protocol" : "pcap", "hpfeed_id" : { "$oid" : "5bd7abf8616a1e2e0d40bb4f" }, "timestamp" : { "$date" : "2018-10-30T00:55:20.572+0000" }, "source_ip" : "123.159.207.27", "source_port" : 59716, "destination_port" : 23, "identifier" : "9ea0b972-dbd3-11e8-be35-42010a800002", "honeypot" : "dionaea" }
There are 1988 data points.

## Any unresolved questions raised by the data collected
I would like to know if there is any other data on the attacks I would be able to get with pluggins and such.
