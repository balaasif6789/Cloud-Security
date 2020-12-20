# Creating a Website in HA

### Create S3 buckets 

### Create a CloudFront Distribution

![](../.gitbook/assets/image%20%2874%29.png)

### Create  Security Groups

#### WebDMZ

![](../.gitbook/assets/image%20%2816%29.png)

#### WebDMZ to RDS

![](../.gitbook/assets/image%20%2857%29.png)

### Create RDS

![](../.gitbook/assets/image%20%2813%29.png)

![](../.gitbook/assets/image%20%28102%29.png)

![](../.gitbook/assets/image%20%2828%29.png)

![](../.gitbook/assets/image%20%2825%29.png)

### Create IAM Role

![](../.gitbook/assets/image%20%2882%29.png)

![](../.gitbook/assets/image%20%2891%29.png)

### Creating an EC2 Instance

![](../.gitbook/assets/image%20%2863%29.png)

Selecting an existing DMZ group

![](../.gitbook/assets/image%20%2859%29.png)

### Installing Wordpress

Install Wordpress 

Upload pictures on the blog. 

The pictures will be available on the wp-content folders 

### Uploading content and code on S3 buckets

Check if our IAM roles for s3 works

aws s3 ls 

aws s3 cp --recursive /var/www/html/wp-content/uploads s3://asifbalasinor-media-2020

aws s3 cp --recursive /var/www/html s3://asifbalasinor-code-2020

aws s3 ls s3://asifbalasinor-code-2020

### Using CloudFront

Configuring URL rewrites in httpd.conf 

![](../.gitbook/assets/image%20%2814%29.png)

Configuring Cloudfront distribution in the .htaccess 

We will use the CloudFront distribution that we have created

![](../.gitbook/assets/image%20%283%29.png)

Sync the files between /var/www/html and the s3 code bucket

![](../.gitbook/assets/image%20%2838%29.png)







