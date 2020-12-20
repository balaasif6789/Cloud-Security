# S3 Security

  
&lt;!--  
 /\* Font Definitions \*/  
 @font-face  
	{font-family:Wingdings;  
	panose-1:5 0 0 0 0 0 0 0 0 0;  
	mso-font-charset:2;  
	mso-generic-font-family:auto;  
	mso-font-pitch:variable;  
	mso-font-signature:0 268435456 0 0 -2147483648 0;}  
@font-face  
	{font-family:"Cambria Math";  
	panose-1:0 0 0 0 0 0 0 0 0 0;  
	mso-font-charset:1;  
	mso-generic-font-family:roman;  
	mso-font-format:other;  
	mso-font-pitch:variable;  
	mso-font-signature:0 0 0 0 0 0;}  
@font-face  
	{font-family:Calibri;  
	panose-1:2 15 5 2 2 2 4 3 2 4;  
	mso-font-charset:0;  
	mso-generic-font-family:swiss;  
	mso-font-pitch:variable;  
	mso-font-signature:-536870145 1073786111 1 0 415 0;}  
 /\* Style Definitions \*/  
 p.MsoNormal, li.MsoNormal, div.MsoNormal  
	{mso-style-unhide:no;  
	mso-style-qformat:yes;  
	mso-style-parent:"";  
	margin-top:0in;  
	margin-right:0in;  
	margin-bottom:8.0pt;  
	margin-left:0in;  
	line-height:107%;  
	mso-pagination:widow-orphan;  
	font-size:11.0pt;  
	font-family:"Calibri","sans-serif";  
	mso-ascii-font-family:Calibri;  
	mso-ascii-theme-font:minor-latin;  
	mso-fareast-font-family:Calibri;  
	mso-fareast-theme-font:minor-latin;  
	mso-hansi-font-family:Calibri;  
	mso-hansi-theme-font:minor-latin;  
	mso-bidi-font-family:"Times New Roman";  
	mso-bidi-theme-font:minor-bidi;}  
a:link, span.MsoHyperlink  
	{mso-style-priority:99;  
	color:\#0563C1;  
	mso-themecolor:hyperlink;  
	text-decoration:underline;  
	text-underline:single;}  
a:visited, span.MsoHyperlinkFollowed  
	{mso-style-noshow:yes;  
	mso-style-priority:99;  
	color:\#954F72;  
	mso-themecolor:followedhyperlink;  
	text-decoration:underline;  
	text-underline:single;}  
p.MsoListParagraph, li.MsoListParagraph, div.MsoListParagraph  
	{mso-style-priority:34;  
	mso-style-unhide:no;  
	mso-style-qformat:yes;  
	margin-top:0in;  
	margin-right:0in;  
	margin-bottom:8.0pt;  
	margin-left:.5in;  
	mso-add-space:auto;  
	line-height:107%;  
	mso-pagination:widow-orphan;  
	font-size:11.0pt;  
	font-family:"Calibri","sans-serif";  
	mso-ascii-font-family:Calibri;  
	mso-ascii-theme-font:minor-latin;  
	mso-fareast-font-family:Calibri;  
	mso-fareast-theme-font:minor-latin;  
	mso-hansi-font-family:Calibri;  
	mso-hansi-theme-font:minor-latin;  
	mso-bidi-font-family:"Times New Roman";  
	mso-bidi-theme-font:minor-bidi;}  
p.MsoListParagraphCxSpFirst, li.MsoListParagraphCxSpFirst, div.MsoListParagraphCxSpFirst  
	{mso-style-priority:34;  
	mso-style-unhide:no;  
	mso-style-qformat:yes;  
	mso-style-type:export-only;  
	margin-top:0in;  
	margin-right:0in;  
	margin-bottom:0in;  
	margin-left:.5in;  
	margin-bottom:.0001pt;  
	mso-add-space:auto;  
	line-height:107%;  
	mso-pagination:widow-orphan;  
	font-size:11.0pt;  
	font-family:"Calibri","sans-serif";  
	mso-ascii-font-family:Calibri;  
	mso-ascii-theme-font:minor-latin;  
	mso-fareast-font-family:Calibri;  
	mso-fareast-theme-font:minor-latin;  
	mso-hansi-font-family:Calibri;  
	mso-hansi-theme-font:minor-latin;  
	mso-bidi-font-family:"Times New Roman";  
	mso-bidi-theme-font:minor-bidi;}  
p.MsoListParagraphCxSpMiddle, li.MsoListParagraphCxSpMiddle, div.MsoListParagraphCxSpMiddle  
	{mso-style-priority:34;  
	mso-style-unhide:no;  
	mso-style-qformat:yes;  
	mso-style-type:export-only;  
	margin-top:0in;  
	margin-right:0in;  
	margin-bottom:0in;  
	margin-left:.5in;  
	margin-bottom:.0001pt;  
	mso-add-space:auto;  
	line-height:107%;  
	mso-pagination:widow-orphan;  
	font-size:11.0pt;  
	font-family:"Calibri","sans-serif";  
	mso-ascii-font-family:Calibri;  
	mso-ascii-theme-font:minor-latin;  
	mso-fareast-font-family:Calibri;  
	mso-fareast-theme-font:minor-latin;  
	mso-hansi-font-family:Calibri;  
	mso-hansi-theme-font:minor-latin;  
	mso-bidi-font-family:"Times New Roman";  
	mso-bidi-theme-font:minor-bidi;}  
p.MsoListParagraphCxSpLast, li.MsoListParagraphCxSpLast, div.MsoListParagraphCxSpLast  
	{mso-style-priority:34;  
	mso-style-unhide:no;  
	mso-style-qformat:yes;  
	mso-style-type:export-only;  
	margin-top:0in;  
	margin-right:0in;  
	margin-bottom:8.0pt;  
	margin-left:.5in;  
	mso-add-space:auto;  
	line-height:107%;  
	mso-pagination:widow-orphan;  
	font-size:11.0pt;  
	font-family:"Calibri","sans-serif";  
	mso-ascii-font-family:Calibri;  
	mso-ascii-theme-font:minor-latin;  
	mso-fareast-font-family:Calibri;  
	mso-fareast-theme-font:minor-latin;  
	mso-hansi-font-family:Calibri;  
	mso-hansi-theme-font:minor-latin;  
	mso-bidi-font-family:"Times New Roman";  
	mso-bidi-theme-font:minor-bidi;}  
.MsoChpDefault  
	{mso-style-type:export-only;  
	mso-default-props:yes;  
	font-family:"Calibri","sans-serif";  
	mso-ascii-font-family:Calibri;  
	mso-ascii-theme-font:minor-latin;  
	mso-fareast-font-family:Calibri;  
	mso-fareast-theme-font:minor-latin;  
	mso-hansi-font-family:Calibri;  
	mso-hansi-theme-font:minor-latin;  
	mso-bidi-font-family:"Times New Roman";  
	mso-bidi-theme-font:minor-bidi;}  
.MsoPapDefault  
	{mso-style-type:export-only;  
	margin-bottom:8.0pt;  
	line-height:107%;}  
@page WordSection1  
	{size:8.5in 11.0in;  
	margin:1.0in 1.0in 1.0in 1.0in;  
	mso-header-margin:.5in;  
	mso-footer-margin:.5in;  
	mso-paper-source:0;}  
div.WordSection1  
	{page:WordSection1;}  
 /\* List Definitions \*/  
 @list l0  
	{mso-list-id:893471424;  
	mso-list-type:hybrid;  
	mso-list-template-ids:554757380 1911431116 67698691 67698693 67698689 67698691 67698693 67698689 67698691 67698693;}  
@list l0:level1  
	{mso-level-start-at:0;  
	mso-level-number-format:bullet;  
	mso-level-text:;  
	mso-level-tab-stop:none;  
	mso-level-number-position:left;  
	text-indent:-.25in;  
	font-family:Wingdings;  
	mso-fareast-font-family:Calibri;  
	mso-fareast-theme-font:minor-latin;  
	mso-bidi-font-family:"Times New Roman";  
	mso-bidi-theme-font:minor-bidi;}  
@list l0:level2  
	{mso-level-number-format:bullet;  
	mso-level-text:o;  
	mso-level-tab-stop:none;  
	mso-level-number-position:left;  
	text-indent:-.25in;  
	font-family:"Courier New";}  
@list l0:level3  
	{mso-level-number-format:bullet;  
	mso-level-text:;  
	mso-level-tab-stop:none;  
	mso-level-number-position:left;  
	text-indent:-.25in;  
	font-family:Wingdings;}  
@list l0:level4  
	{mso-level-number-format:bullet;  
	mso-level-text:;  
	mso-level-tab-stop:none;  
	mso-level-number-position:left;  
	text-indent:-.25in;  
	font-family:Symbol;}  
@list l0:level5  
	{mso-level-number-format:bullet;  
	mso-level-text:o;  
	mso-level-tab-stop:none;  
	mso-level-number-position:left;  
	text-indent:-.25in;  
	font-family:"Courier New";}  
@list l0:level6  
	{mso-level-number-format:bullet;  
	mso-level-text:;  
	mso-level-tab-stop:none;  
	mso-level-number-position:left;  
	text-indent:-.25in;  
	font-family:Wingdings;}  
@list l0:level7  
	{mso-level-number-format:bullet;  
	mso-level-text:;  
	mso-level-tab-stop:none;  
	mso-level-number-position:left;  
	text-indent:-.25in;  
	font-family:Symbol;}  
@list l0:level8  
	{mso-level-number-format:bullet;  
	mso-level-text:o;  
	mso-level-tab-stop:none;  
	mso-level-number-position:left;  
	text-indent:-.25in;  
	font-family:"Courier New";}  
@list l0:level9  
	{mso-level-number-format:bullet;  
	mso-level-text:;  
	mso-level-tab-stop:none;  
	mso-level-number-position:left;  
	text-indent:-.25in;  
	font-family:Wingdings;}  
ol  
	{margin-bottom:0in;}  
ul  
	{margin-bottom:0in;}  
--&gt;  


EC2

è Firewall

è Security groups

è EC2 authentication \( Password based or SSH key based \)

EBS

è Volume encryption

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

