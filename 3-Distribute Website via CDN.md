# Distribute Website via CloudFront

1. From the CloudFront dashboard, click “Create a CloudFront Distribution”.
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/d0982025-b685-4266-a567-265495255446)

2. Enter the s3 bucket website endpoint as origin domain as shown below
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/510feae8-6ae3-44d6-8798-186625ac9009)

3. Leave the defaults configurations for the rest of the options, and click 'Create distribution'. It navigate to newly created distribution with status as **'Deploying'**
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/67d4ae23-b95c-4ba2-8f68-8d4b27b130bf)

4. It may take up to 10 minutes for the CloudFront Distribution to deploy, deployment will be sucessfully once the status change to enable
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/24b0c11d-ab99-4f51-a6e8-02ba8df1c916)

5. Now copy the endpoint URL for your CloudFront distribution found in the “Domain Name” column.
![image](https://github.com/sateeshfrnd/Deploy-Static-Website-on-AWS/assets/8160366/b36491f5-0734-4a1f-b065-0d028d425496)

> Here, the Domain Name value is **d2133uyibrvkwk.cloudfront.net**
