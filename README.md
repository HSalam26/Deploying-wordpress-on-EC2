# Deploying WordPress Server on AWS EC2 Instance

Follow these steps to deploy a WordPress server on an AWS EC2 instance:

## Step 1: AWS Login
- Begin by logging into your AWS account.

## Step 2: Create an EC2 Instance
- Navigate to the EC2 service in the AWS Management Console.
- Click "Launch Instance."
- Choose an Amazon Machine Image (AMI):
  - In the AMI marketplace, search for "WordPress."
  - Select "WordPress certified by Bitnami."
- Configure Instance Type:
  - Opt for the "t2.micro" instance type.
- Configure Security Settings:
  - Either use an existing key pair or create a new one.
- Configure Storage:
  - Modify the storage size to 30GB (within the AWS Free Tier limits).
- Review and Launch:
  - Carefully review your instance settings and click "Launch."

## Step 8: Verify the WordPress Server
- Once the instance is running, note its public IP address.
- Open your web browser and paste the public IP address.
- Confirm that the WordPress server is operational.

## Step 9: Access the WordPress Admin Panel
- To access the WordPress login page, add "/wp-admin" to the end of the URL (e.g., `http://<public-ip>/wp-admin`).

## Step 10: Retrieve Username and Password
- Access the AWS Management Console.
- Navigate to the EC2 dashboard.
- Select your WordPress server instance.
- Click on "Actions" > "Instance Settings" > "Get System Log."

## Step 11: Find Username and Password
- Scroll through the system logs until you locate the WordPress username and password.

## Step 12: Log In to WordPress
- Use the retrieved username and password to log in to the WordPress dashboard.

**Important:** Don't forget to terminate or stop your instances when you are done to avoid unnecessary charges and maintain the security of your resources.

Congratulations! You have successfully deployed a WordPress server on an AWS EC2 instance.
