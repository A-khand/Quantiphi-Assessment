AWS
 Ans 3.
step for Ec2
1. go to aws service click Ec2
2.click launch instant
3. choose AMi
4. choose instatnt type
5.click configure instance
6.click add storage
7.add tag
8.configure security group(add network type,ip,protocol )
9.click review and launch
10 create and download key pair
11.click launch instance



ANS 5.
vpc
1 go to console create vpc
2.launch vpc
3. give the name for vpc
4. create vpc
5. click sunnate
6. give name for subnate select zone and vpc
7. create subnate
8. create internet gatway
9. add gatway to vpc
10. add route table to public subnate
11 add name and vpc
12 go to route table select public route table
13 click subnate association
14  select public rt and with public net


Ans.1
iam for s3 only
1. go to iam
2. go to policy
3. create you own policy
4. go to json
5. give th name,give the description
6. attach json file


{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Action": [
                        "s3:GetBucketLocation",
                        "s3:ListAllMyBuckets"
                      ],
            "Resource": "arn:aws:s3:::*"
        },
        {
            "Effect": "Allow",
            "Action": "s3:*",
            "Resource": [
                "arn:aws:s3:::YOUR-BUCKET",
                "arn:aws:s3:::YOUR-BUCKET/*"
            ]
        }
    }
6. create group
7. give group name
8 attech policy
9.click next
10 go to group review screen
11 click create group
12. select group and go to action for add  user to group
13 add user

Ans4
s3 bucket for static website
1. go to s3
2. click on create bucket
3 add name to bucket
4 clicke on newly create bucket
5.  click on upload and upload your website
6. go to parmission
7 dissable public access
8.  go to bucket policy
9. add file
{
  "Version":"2012-10-17",
  "Statement":[
    {
      "Sid":"AddPerm",
      "Effect":"Allow",
      "Principal": "*",
      "Action":["s3:GetObject"],
      "Resource":["arn:aws:s3:::examplebucket/*"]
    }
  ]
10. go in properties
11. go to static website hosting
12 select use this bucket for website hosting
13 give a entry point page name
14  click save
15 click again on static website hosting
16 in top link is availabe copy this link in your browser


Qus2.
What will be the outcome of this IAM Policy?
{
"Version": "2012-10-17",
"Statement": [{
"Action": "ec2:*",
"Resource": "*",
"Effect": "Allow"
},
{
"Action": "*",
"Resource": "*",
"Effect": "Deny"
}
]
}
  ans2.
   all user take all action on  ec2 and it's resources but all user not access the all service and it's recources
all user can only access ec2 and it's resources

