---
title: "Getting Started with Terraform – Simple EC2 Example"
description: "Learn how to launch your first EC2 instance using Terraform – step by step in Roman Urdu style."
pubDate: "Jul 31 2025"
heroImage: "/blog-placeholder-3.jpg"
---

Assalamualaikum doston! 👋  
Aaj ka yeh mera pehla blog post hai jahan hum **Terraform ka basic use case** dekhtay hain – ek simple EC2 instance deploy karna on AWS.

## 🔧 Terraform Kya Hai?

Terraform ek Infrastructure as Code (IaC) tool hai jo humein cloud resources jaise ke EC2, VPC, S3, waghera ko code ki form mein manage karne deta hai. Yani infrastructure ko manually create karne ki bajaye, hum `.tf` files ke zariye define karte hain.

---

## 📁 Basic Terraform Project Structure

```bash
terraform-ec2/
├── main.tf
├── variables.tf
└── terraform.tfvars
````

---

## ✍️ Step 1: `main.tf` – EC2 Configuration

```hcl
provider "aws" {
  region = "us-east-1"
}

resource "aws_instance" "example" {
  ami           = "ami-0c55b159cbfafe1f0" # Amazon Linux 2
  instance_type = "t2.micro"

  tags = {
    Name = "MyFirstEC2"
  }
}
```

---

## ✍️ Step 2: `variables.tf` – Variables Define Karna (Optional)

```hcl
variable "region" {
  default = "us-east-1"
}
```

---

## ✍️ Step 3: Commands to Deploy

```bash
terraform init       # Initialize project
terraform plan       # Check what will be created
terraform apply      # Deploy the EC2 instance
```

Apply karne ke baad AWS Console pe jakay EC2 section mein aapko aapka instance nazar aayega.

---

## 🧹 Cleanup (Delete Resources)

```bash
terraform destroy
```

---

## 🧠 Final Words

Yeh sirf basic example tha. Terraform ka power tab samajh aata hai jab aap VPCs, Subnets, Security Groups, aur autoscaling waghera automate karte hain.

Agle posts mein hum yeh sab explore karenge, step by step – aur har cheez ko **simple Roman Urdu** mein samjhayenge.

Shukriya! 💻✨
**\~ Rao Shahzaib**

```

---

### ✅ Highlights:
- Clear and simple for beginners.
- Explained in a Roman Urdu + English mix, as per your style.
- Practical Terraform EC2 example.
- Room to expand in future posts.

Want me to generate the code files (`main.tf`, `variables.tf`, `terraform.tfvars`) as downloads or GitHub repo format?
```
