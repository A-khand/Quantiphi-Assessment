Q1.Steps to create VPC and subnets

1.Open the VPC networks page in GCP console
2.Click on Create VPC network
3.Enter a Name for the network
4.Choose Automatic or Custom for the Subnet creation mode
5.If Custom, provide Name, Region, IP Address Range, Access and Flow Logs
6.Choose the Dynamic routing mode for the VPC network
7.Click Create

Q2.Steps to create a service account and add IAM roles which grants access to GCE and GCS only
Create a Service Account

1.Open the Service Accounts page in the Cloud Console
2.Click on Select a project, choose your project, and click Open
3.Click on Create Service Account
4.Enter a service account name, an optional description, select a role you wish to grant to the service account and then click Save

Granting roles to a service account
1.Open the IAM & Admin page in the GCP Console
2.Click on Select a project, choose a project, and click on Open
3.Identify the service account to which you want to add a role
4.Select one or more roles to apply to the service account
5.Click on Save to apply the roles

Q3.Steps to create bucket and transfer files from local to GCS using gsutil

Create Bucket
1.Open the Cloud Storage browser in the GCP Console
2.Click Create bucket, enter Name, Default Storage Class, Control Access
3.Click Done

transfer files from local to GCS using gsutil
gsutil cp Desktop/kitten.png gs://my-awesome-bucket

Q4.Steps to create GCE VM and deploy nginx

Create GCE VM
1.Go to the VM instances page
2.Select your project and click on Continue
3.Click the Create instance button and specify a Name for your instance
4.Select a Machine configuration for your instance
5.In the OS images tab, choose an image
6.To permit HTTP or HTTPS traffic to the VM instance, select Allow HTTP traffic or Allow HTTPS traffic
7.Click the Create button to create and start the instance

Deploy nginx
1.Access the NGINX Plus page in Google Marketplace
2.Click on the LAUNCH ON COMPUTE ENGINE button
3.The Select or create a project window opens
4.Select a Project from the dropdown, click on Create button
5.In the Configure & Deploy window, enter or select appropriate values for zone, machine type and so on
6.Click on Deploy button
7.Click on Create button
