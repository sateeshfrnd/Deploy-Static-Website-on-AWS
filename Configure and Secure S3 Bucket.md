# Configure S3 Bucket and Secure Bucket via IAM

## Secure Bucket via IAM
1. Click on the “Permissions” tab
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/3311d794-d70b-4dd8-8d5e-ffef2d3c89af)

2. Scroll down to edit the *'Bucket Policy'* section, default it shows empty bucket policy.
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/8ed17c50-baa7-4e68-859d-d9aec081aea8)

3. Click on the Edit button and enter the following bucket policy and click *'Save'*
```
{
  "Version":"2012-10-17",
  "Statement":[
    {
      "Sid":"AddPerm",
      "Effect":"Allow",
      "Principal": "*",
      "Action":["s3:GetObject"],
      "Resource":["arn:aws:s3:::your-website/*"]
    }
  ]
}
```
> **Note:** Replacing your-website with the name of your bucket

![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/c0fd7a6f-edf0-46cb-90df-aecc47841245)


4. Our Bucket policy is updated 
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/a4fedb59-6329-4d7d-83bf-3a3cc205211a)

> You will see warnings about making your bucket public, but this is required for static website hosting.



## Configure S3 Bucket
1. Go to the Properties tab
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/e9f3163d-7861-4e66-9ab4-d8a1aea9f980)

2. Scroll down to edit the Static website hosting section and Click on the *'Edit'* button
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/416db0af-76ea-4018-8e49-db838b65de21)

3. Enable the static website hosting, and provide the home page and error page of your website and click 'Save Changes'
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/2fe9802b-cb23-4753-b52b-546efa767dbf)

4. After saving check again the Static website hosting section, now you can able to view the website endpoint as shown below
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/2bd6a2a9-53ad-4653-be8e-b7a4a65a4558)

5. Copy the website endpoint for future use
> http://my-static-website-jj.s3-website-us-east-1.amazonaws.com/
