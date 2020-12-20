# Load Balancers

1. Start with creating an EC2 instance. We will be launching 2 different instances in 2 different Availability Zones.
2. Use a Bootstrap script to create a webserver 1
3. We will create another EC2 instance. This will be placed in a sepeate AZ.
4. Again we will use a bootstrap script to create a webserver2
5. Browse to the IP from the browser and ensure that both the servers are running. 

### Creating an ELB

1. Screen 1

![](../.gitbook/assets/image%20%28109%29.png)

2. Screen 2 . Selecting the Web DMZ

![](../.gitbook/assets/image%20%2892%29.png)

3. Health Check

![](../.gitbook/assets/image%20%2824%29.png)

4. Adding EC2 instances

![](../.gitbook/assets/image%20%2834%29.png)

We see that the instances are now in service

![](../.gitbook/assets/image%20%2881%29.png)

**Note below that we have not been assigned an IP address for ELB. We have been given only a DNS name**

![](../.gitbook/assets/image%20%2877%29.png)

Browse to the DNS name 

![](../.gitbook/assets/image%20%2846%29.png)

Keep hitting refresh and we see that it oscillates between server 1 and server 2

![](../.gitbook/assets/image%20%2812%29.png)

### Creating a Web Application Load Balancer

#### Creating a Resource Group

![](../.gitbook/assets/image%20%2818%29.png)

#### Adding Targets to the Resource Group

![](../.gitbook/assets/image%20%2868%29.png)

Click Edit, select the Target instances and add to registered targets

![](../.gitbook/assets/image%20%2822%29.png)

Create an Application LB 

![](../.gitbook/assets/image%20%2854%29.png)

![](../.gitbook/assets/image%20%2887%29.png)

![](../.gitbook/assets/image%20%2867%29.png)

![](../.gitbook/assets/image%20%2862%29.png)

![](../.gitbook/assets/image%20%2869%29.png)

If we go over to our ALB using the dns name 

![](../.gitbook/assets/image%20%2852%29.png)

Refresh and we get the page

![](../.gitbook/assets/image%20%2894%29.png)

### Additional Concepts 

#### No Cross Zone Load Balancer

Load Balancing is done in the same availability zone

![](../.gitbook/assets/image%20%2820%29.png)

#### Cross Zone Load Balancer 

Load balancing is done across different availability zones

![](../.gitbook/assets/image%20%2827%29.png)





