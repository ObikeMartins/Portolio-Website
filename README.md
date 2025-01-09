# Personal Portfolio Website

This project demonstrates how to create and deploy a personal portfolio website using AWS services like S3, Route 53, and CloudFront (optional for SSL). The website is hosted on a custom domain (`obikemartins.com`).

## Technologies Used
- **HTML**: For the structure of the portfolio.
- **CSS**: For styling the portfolio page.
- **JavaScript**: (Optional) For adding interactivity.
- **AWS S3**: For hosting the static website.
- **AWS Route 53**: For managing DNS and pointing the custom domain to S3.
- **CloudFront (Optional)**: For SSL and HTTPS support.

## Setup Guide

### Step 1: Prepare Website Files
1. Create `index.html`, `style.css`, and `script.js` files.
2. Customize these files for your personal portfolio.

### Step 2: Set Up AWS S3 for Static Website Hosting
1. Log in to AWS Console and navigate to S3.
2. Create a new S3 bucket named `martinsobike.com`.
3. Upload `index.html`, `style.css`, and `script.js` files to the S3 bucket.
4. Enable static website hosting in the bucket settings.

### Step 3: Configure Route 53 to Point to S3 Bucket
1. Navigate to Route 53 and create a hosted zone for `martinsobike.com`.
2. Create an Alias record to point to your S3 bucket's website endpoint.

### Step 4: Optional - Set Up SSL with CloudFront
1. Request an SSL certificate from AWS Certificate Manager (ACM).
2. Set up a CloudFront distribution to serve your website over HTTPS.
3. Update DNS records in Route 53 to point to CloudFront.

### Step 5: Testing
1. Visit `http://martinsobike.com` to see your portfolio.
2. If SSL is set up, use `https://martinsobike.com`.

## Conclusion
This guide shows how to host a static website using AWS S3 and Route 53 with a custom domain. For added security, CloudFront with SSL support can be configured to serve the website over HTTPS.
