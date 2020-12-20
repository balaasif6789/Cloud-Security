# EC2

### EBS Types

![](../.gitbook/assets/image%20%28108%29.png)

### IAM Roles with EC2 

Creating a Role for EC2

![](../.gitbook/assets/image%20%2826%29.png)



![](../.gitbook/assets/image%20%2819%29.png)

![](../.gitbook/assets/image%20%286%29.png)

Attaching IAM role to the EC2 instance.

![](../.gitbook/assets/image%20%2836%29.png)

![](../.gitbook/assets/image%20%2886%29.png)

The JSON file of the IAM Role

![](../.gitbook/assets/image%20%2844%29.png)

### Boot Strap scripts - EC2 Instance 

While creating an instance you can automate certain tasks which would be performed manually on the EC2 instance. This can be done with the help of boot strap scripts.

This can be done while creating an EC2 instance. In the configure screen we can add a bash script as shown below. The below scripts install apache and creates an s3 bucket. 

![](../.gitbook/assets/image%20%2837%29.png)

curl http://169.254.169.254/latest/user-data

![](../.gitbook/assets/image%20%2829%29.png)

### EC2 Metadata

![](../.gitbook/assets/image%20%2848%29.png)

Viewing IPv4 and Hostname

![](../.gitbook/assets/image%20%28105%29.png)

### AMAZON Elastic File System \(EFS\) 

Create an EFS using the default settings from the console

**Enable encryption**

Create a EC2 instance. **Set the number of instances to 2**

Enter the bootstrap script 

![](../.gitbook/assets/image%20%282%29.png)

Edit the inbound rules of the default security group. The web server we setup on the instance will need to communicate with the EFS file system over NFS i.e port 2049. We set up a firewall rule accordingly in the Security Groups.

![](../.gitbook/assets/image%20%2849%29.png)



\*\*\*\*

