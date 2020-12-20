# S3 Buckets -Security

##  Bucket Access  to public

By default access is not public

![](../.gitbook/assets/image%20%2850%29.png)

Making bucket public

![](../.gitbook/assets/image%20%2856%29.png)

 Make the individual objects public

![](../.gitbook/assets/image%20%2875%29.png)

## Enable Server Side Encryption for S3

One SSE is enabled, only added objects  post the activation will be automatically encrypted, objects added before will have to be encrypted manually.

![](../.gitbook/assets/image%20%2811%29.png)

If afterwards SSE is disabled at the bucket level, even then SSE for the objects created in the previously encrypted bucket will continue to remain encrypted.

[https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html)

## MFA Delete  on bucket

MFA delete can only be activated from the cli and not from the console

https://docs.aws.amazon.com/AmazonS3/latest/dev/Versioning.html\#MultiFactorAuthenticationDelete

