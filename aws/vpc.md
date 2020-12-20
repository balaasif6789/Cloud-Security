# VPC

### Creating VPC

#### Creating the VPC

![](../.gitbook/assets/image.png)

#### Creating a Subnet

![](../.gitbook/assets/image%20%2823%29.png)

#### Auto Assigning IP Addresses

![](../.gitbook/assets/image%20%2832%29.png)

Click on Auto-Assign IP4

#### **Creating an Internet Gateway\(IGW\)**

 Create an IGW. All it takes is adding a name. 

By default the IGW has the status of **Detached**

![](../.gitbook/assets/image%20%2842%29.png)

We need to attach the IGW to our created VPC. Select the IGW , go to action and select attach to VPC 

![](../.gitbook/assets/image%20%2845%29.png)

#### Create a Separate Route Table

We create a separate route table. 

![](../.gitbook/assets/image%20%2843%29.png)

Edit routes in the route table

![](../.gitbook/assets/image%20%2860%29.png)

We now get a Route out to the internet. Any sub nets associated with this route table will be publicly available. 

![](../.gitbook/assets/image%20%2890%29.png)

We will go to Subnet Associations and click on Edit Subnets. We will add the subnet 10.0.1.0 to our Public Route table

![](../.gitbook/assets/image%20%2865%29.png)

![](../.gitbook/assets/image%20%281%29.png)

We will create 2 EC2 instances. While creating the instance we will select the VPC that we created. For the public instance we will select the public subnet and for the private instance we will select the private subnet. 

\*\*\*\*

