# Access Website

## Access Website via CloudFront domain name 

Copy CloudFront domain **(without appending /index.html at the end)** and open in web browser then the content of the default home-page will show as below:
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/38c73014-8887-49b0-b837-d362132baa26)

In the above you can see the page url as CloudFront domain name **https://d2133uyibrvkwk.cloudfront.net/**

## Access Website via static website-endpoint 
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/624922db-384a-4a90-8f2c-41cfdd02792d)

In the above you can see the page url as static website-endpoint **http://my-static-website-jj.s3-website-us-east-1.amazonaws.com/**


## Access Website via S3 object URL 
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/e73cb39e-2aa4-4548-9efd-3e66dd00204e)

In the above you can see the page url as S3 object URL **https://my-static-website-jj.s3.amazonaws.com/index.html**



> **All three links: CloudFront domain name, S3 object URL, and website-endpoint will show you the same 'index.html' content.**
