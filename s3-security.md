# S3 Security

S3

è Bucket Access  to public

By default access is not public

![](file:///C:\Users\bounty\AppData\Local\Temp\msohtmlclip1\01\clip_image002.jpg)

Making bucket public

![](file:///C:\Users\bounty\AppData\Local\Temp\msohtmlclip1\01\clip_image004.jpg)

![](file:///C:\Users\bounty\AppData\Local\Temp\msohtmlclip1\01\clip_image006.jpg)

 Make the individual objects public

![](file:///C:\Users\bounty\AppData\Local\Temp\msohtmlclip1\01\clip_image007.jpg)

Enable Server Side Encryption for S3

![](file:///C:\Users\bounty\AppData\Local\Temp\msohtmlclip1\01\clip_image009.jpg)

One SSE is enabled, only added objects  post the activation will be automatically encrypted, objects added before will have to be encrypted manually.

![](file:///C:\Users\bounty\AppData\Local\Temp\msohtmlclip1\01\clip_image011.jpg)

If afterwards SSE is disabled at the bucket level, even then SSE for the objects created in the previously encrypted bucket will continue to remain encrypted.

[https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html)

MFA Delete  on bucket

https://docs.aws.amazon.com/AmazonS3/latest/dev/Versioning.html\#MultiFactorAuthenticationDelete

CloudTrail on S3

Amazon S3 is integrated with AWS CloudTrail, a service that provides a record of actions taken by a user, role, or an AWS service in Amazon S3. CloudTrail captures a subset of API calls for Amazon S3 as events, including calls from the Amazon S3 console and from code calls to the Amazon S3 APIs. If you create a trail, you can enable continuous delivery of CloudTrail events to an Amazon S3 bucket, including events for Amazon S3. If you don't configure a trail, you can still view the most recent events in the CloudTrail console in **Event history – from the AWS Website**

https://docs.aws.amazon.com/AmazonS3/latest/dev/cloudtrail-logging.html99

