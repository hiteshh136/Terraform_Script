Terraform Script for create 2 aws instances with attach s3 bucket and rds database with load balancing
Step 1: Clone the given repository.
Step 2: Configure your aws credentials using aws configure.
Step 3: run terraform init command in 01_aws_backend
Step 4: run terraform apply command in 01_aws_backend to apply changes in your linked aws account.

Step 5: run terraform init command in 02_web_app
Step 6: run terraform apply command in 02_web_app to apply changes in your linked aws account.

// File 01_aws_backend will create: s3_bucket, s3_bucket_versioning, s3_bucket_server_side_encryption_configuration, dynamodb_table
// File 02_web_app will create: aws_instance, s3_bucket, s3_bucket_versioning, default_vpc, subnet_ids, security_group, security_group_rule, load_balancer, lb_target_group, security_group_rule,route53_zone, route53_record, db_instance