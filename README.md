
Easily set up your AWS infrastructure with this module! It handles everything for you:

- 🚀 **Application Load Balancer (ALB)**  
- 📈 **Auto Scaling Groups (ASG)**  
- 🛠 **Launch Templates**  
- 🎯 **Target Groups**  
- 🗂 **S3 Buckets**  
- 💻 **EC2 Instances**  
- 🔧 **Custom AMI setups**  

## What Does It Do?

This module creates the backbone of your AWS environment:  
- **Load Balancing**: ALB spreads traffic across multiple instances.  
- **Auto-Scaling**: Automatically adjust EC2 instances based on demand.  
- **Storage**: S3 buckets with optional encryption and lifecycle rules.  
- **Custom EC2 Setup**: Use your own AMIs or stick with AWS defaults.  

## Getting Started 🚀

### Requirements  
1. **AWS CLI** installed and configured.  
2. **Terraform 1.x+** installed.  
3. **IAM Permissions** to create EC2, S3, and ALB resources.  

### Example Use

```hcl
module "aws_setup" {
  source        = "./aws-infra-module"
  region        = "us-east-1"
  vpc_id        = "vpc-1234abcd"
  subnet_ids    = ["subnet-1111abcd", "subnet-2222abcd"]
  bucket_name   = "my-app-storage"
  instance_type = "t3.medium"
  ami_id        = "ami-12345abcde"
}
```

### Outputs  
- ✅ ALB DNS Name  
- ✅ S3 Bucket Name  
- ✅ Instance IDs  

## Why Use This Module?

- **Simple**: Just plug and play.  
- **Powerful**: Scales automatically and supports custom setups.  
- **Reliable**: Built with best practices in mind.  

---

For more, visit my blog: [docs.ahmadraza.in](https://docs.ahmadraza.in)  
