# Cloudreach3tier


![GCP 3 tier-1](https://user-images.githubusercontent.com/105651061/168604227-a4ddcbf3-fbf3-439d-88c5-7d1372bf1702.png)

I have hosted the application on Google cloud.

For 3 tier architecture
Created one VPC
and in VPC created 3 subnets

Hosted the webservers in subnet1.
Application in Subnet2.
DB in Subnet3.

Created a load balancer on top of Webservers, to manage the load routing.
Assuming webservers will be acted as load balancer to App Servers, if not case needed another load balancer.

Webserver is opened on Port 443
App server is opened on port 8080
DB on 3306

Created private IP for google cloud sql and allowed only App server IP range.
Created Managed instance groups for Web and App servers.
