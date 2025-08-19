# s3StaticWebsite


# Steps to Host a Static Website on Amazon S3

## 1. Create an S3 Bucket
Start by creating an S3 bucket to store your website files.  
- The bucket name must be **globally unique** across all AWS accounts.

## 2. Configure Bucket for Static Website Hosting
- In the S3 bucket properties, enable **static website hosting**.
- Specify the default index document (e.g., `index.html`) and optional error document (e.g., `error.html`).

## 3. Upload Website Files
- Upload your static website files (HTML, CSS, JS, images, etc.) to the S3 bucket.
- Set appropriate permissions (e.g., `public-read`) for the objects to make them publicly accessible.

## 4. Enable Public Access
- Allow public access to the S3 bucket and its objects by configuring the **bucket policy** or **Access Control Lists (ACLs)**.

## 5. Configure DNS (Optional)
- If you want to use a custom domain (e.g., `www.yourdomain.com`), set up a DNS record using **Route 53** or another DNS provider.
- This step is optional if you're using the default S3 website endpoint.

## 6. Test the Website
- Once setup is complete, test your static website by accessing it through the **S3 bucket website URL** or your **custom domain**.
