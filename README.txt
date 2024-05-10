Name: Israel Nteile
Alt School ID: ALT/SOE/023/2691

Hosting a static website using s3 bucket (private bucket) but
with public read policy assigned, using cloud front for CND.  
solution

1. Create bucket and give a simple name .e.g myinteriorapp
2. Disable bucket key and click create bucket
3. Click on the bucket name and click on upload files
4. Click on add files, select the files and folders
5. Click upload to upload them. Before you click upload, you can adjust the permissions or leave it default.
6. Click on service and look for cloudfront 
8. Click on create distribution -> under origin domain, select the bucket name.
9. Under access, select origin access cotrol which is recommeded
10. Click on create control setting -> click on create on the dialog box
11. Click on create distriution then. At the top, click to copy bucket policy, click on edit bucket policy, and paste it there. and save changes 
12. Next under the bucket properties -> locate static wesite hosting and click edit -> click on enable -> under index document, type index.html and click on save
13. Under cloud front, click refresh to see if it has finish deploying. once it finish, you will see enabled with date and time reference   
14. To access the webpage on broswer, type the cloudfront url/index.html    


Homepage Link
https://d1weo3h61xoi49.cloudfront.net/index.html

CloudFront ID
EKRQ73VJRE9UP

S3 Bucket 
arn:aws:s3:::myinteriorapp
https://eu-north-1.console.aws.amazon.com/s3/buckets/myinteriorapp?region=eu-north-1&bucketType=general