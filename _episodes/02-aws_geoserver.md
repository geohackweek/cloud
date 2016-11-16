---
title: "Geoserver for sharing geospatial data on AWS"
teaching: 20
exercises: 0
questions:
- "How do I quickly share a large amount of geospatial data between my collaborators?"
objectives:
- "Understand how cloud computing can help you disseminate your data quickly" 
- "Use Amazon Web Services to spin up a quick instance of an open source server for geospatial data (Geoserver)"
- "Understand potential use cass"
keypoints:
- AWS s3, EC2 and EBS
- Creating AMIs
---

### Using the AWS s3 bucket 

* Allows a bunch of people to dump in their data instead of giving every one access to your virtual machine
* s3 serves as backup - you can also move really old data that you'll probably never access to Glacier storage
* Use sync to transfer data from s3 to EBS 

### Set up Geoserver

* install Apache Tomcat (for stability, use Tomcat7)
* install PostGres and Post GIS
* install geoserver

### Costing
* s3 bucket - 3TB ~ $1100/year
* Glacier - 5TB ~ $450/year
* ec2 Instance ~ $1000/year
* Total cost ~ $2550/year




