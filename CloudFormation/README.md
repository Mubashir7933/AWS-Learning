# 📦 AWS CloudFormation - Infrastructure as Code (IaC)

Welcome to the CloudFormation section of my AWS Learning Journey!  
Here you'll find simplified explanations and examples of how CloudFormation helps manage cloud infrastructure using code.

---

## 🧠 What is AWS CloudFormation?

**AWS CloudFormation** is a service that lets you define your entire cloud setup — like servers, databases, storage, and networking — in a single text file (YAML or JSON).  
You write this "template" once, and AWS builds everything for you automatically. This is called **Infrastructure as Code**.

---

## ⚙️ What is Infrastructure as Code (IaC)?

> "Instead of clicking around to create servers and databases, you write code that does it for you — automatically and repeatably."

With IaC:
- You treat infrastructure like software code.
- You can version it, track it, and reuse it.
- It saves time, reduces human error, and helps with automation.

---

## 🔧 Example CloudFormation Template (YAML)

This creates a basic EC2 instance:

```yaml
Resources:
  MyEC2Instance:
    Type: AWS::EC2::Instance
    Properties:
      InstanceType: t2.micro
      ImageId: ami-0abcd1234efgh5678
