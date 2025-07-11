# Introduction
This project focuses on applying core cryptographic principles to enhance data confidentiality within an AWS environment. The central objective is to secure files hosted on an Amazon EC2 instance by implementing encryption and decryption workflows aligned with data protection standards. By configuring the AWS Encryption CLI and utilizing AWS Key Management Service (KMS), the solution enables users to create encryption keys, encrypt plaintext files, and securely decrypt ciphertext. Through this hands-on implementation, the project demonstrates a proactive approach to safeguarding sensitive information using AWS-native services.
Key Objectives:
- Generate and manage encryption keys with AWS KMS
- Set up and use the AWS Encryption CLI
- Encrypt plaintext and decrypt ciphertext
##  Creating an AWS KMS key
This step initiates the encryption workflow by generating a cryptographic key with AWS Key Management Service (KMS). AWS KMS enables the creation, storage, and management of secure keys across multiple AWS services. The generated key will be used in subsequent steps to encrypt and decrypt data within an EC2-hosted environment.
<img width="907" height="607" alt="Screenshot 2025-07-10 at 22 07 21" src="https://github.com/user-attachments/assets/6cbccd4a-8c4b-4fea-b72c-ce42babb9594" />
<img width="1440" height="695" alt="Screenshot 2025-07-10 at 22 12 43" src="https://github.com/user-attachments/assets/24fda8f6-87e4-4570-a815-49e6247f1ff6" />
