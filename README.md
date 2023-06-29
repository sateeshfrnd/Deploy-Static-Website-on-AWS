# Deploy-Static-Website-on-AWS

## Project Overview
The cloud is perfect for hosting static websites that only include HTML, CSS, and JavaScript files that require no server-side processing. The whole project has two major intentions to implement:

- Hosting a static website on S3 and
- Accessing the cached website pages using CloudFront content delivery network (CDN) service. Recall that CloudFront offers low latency and high transfer speeds during website rendering.

```
Note that Static website hosting essentially requires a public bucket, whereas the CloudFront can work with public and private buckets.
```
## Website Files
The files included are: 
| File      | Description |
| ----------- | ----------- |
| index.html      | TThe Index document for the website.      |
| error.html      | TThe Error Index document for the website.      |
| /img            | The background image file for the website.       |
| /vendor         | Bootssrap CSS framework, Font, and JavaScript libraries needed for the website to function     |
| /css            | CSS files for the website       |



In this project, you will deploy a static website to AWS by performing the following steps:

- [You will create a public S3 bucket and upload the website files to your bucket.](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/blob/main/1-Create%20S3%20Bucket%20and%20upload%20website%20files.md)
- [You will configure the bucket for website hosting and secure it using IAM policies.](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/blob/main/2-Configure%20and%20Secure%20S3%20Bucket.md)
- [You will speed up content delivery using AWS’s content distribution network service, CloudFront.](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/blob/main/3-Distribute%20Website%20via%20CDN.md)
- [You will access your website in a browser using the unique CloudFront endpoint.](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/blob/main/4-Access%20Website.md)

