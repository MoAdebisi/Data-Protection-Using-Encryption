# Introduction
This project focuses on applying core cryptographic principles to enhance data confidentiality within an AWS environment. The central objective is to secure files hosted on an Amazon EC2 instance by implementing encryption and decryption workflows aligned with data protection standards. By configuring the AWS Encryption CLI and utilizing AWS Key Management Service (KMS), the solution enables users to create encryption keys, encrypt plaintext files, and securely decrypt ciphertext. Through this hands-on implementation, the project demonstrates a proactive approach to safeguarding sensitive information using AWS-native services.
Key Objectives:
- Generate and manage encryption keys with AWS KMS
- Set up and use the AWS Encryption CLI
- Encrypt plaintext and decrypt ciphertext
##  Creating an AWS KMS key
This step initiates the encryption workflow by generating a cryptographic key with AWS Key Management Service (KMS). AWS KMS enables the creation, storage, and management of secure keys across multiple AWS services. The generated key will be used in subsequent steps to encrypt and decrypt data within an EC2-hosted environment.
<img width="907" height="607" alt="Screenshot 2025-07-10 at 22 07 21" src="https://github.com/user-attachments/assets/6cbccd4a-8c4b-4fea-b72c-ce42babb9594" />
Symmetric encryption uses the same key to encrypt and decrypt data, which makes it fast and efficient to use.
<img width="1440" height="695" alt="Screenshot 2025-07-10 at 22 12 43" src="https://github.com/user-attachments/assets/24fda8f6-87e4-4570-a815-49e6247f1ff6" />
## Configuring the File Server instance
This step of the project focuses on preparing the EC2 environment to leverage AWS cryptographic services. The primary goal is to configure AWS credentials on the EC2 file server instance, enabling secure interaction with AWS Key Management Service (KMS). Following credential setup, the AWS Encryption Command Line Interface (CLI) will be installed to facilitate encryption and decryption operations. Together, these steps establish the foundational tools required to perform secure key-based data transformations directly from the EC2 instance.
<img width="2618" height="1420" alt="image" src="https://github.com/user-attachments/assets/642c03f7-02f5-4bae-a338-2b0d8b19f00a" />
AWS credentials is now configured and the AWS Encryption CLI is installed to enable secure data encryption with KMS.
## Encrypt and decrypt data
This task involves creating a mock sensitive file, encrypting its contents using AWS KMS and the Encryption CLI, and then decrypting the file to verify the data remains secure yet accessible.
<img width="2880" height="1026" alt="image" src="https://github.com/user-attachments/assets/fffba6f9-d245-44e4-b74f-06ec0e0269cd" />
The encryption and decryption process begins with plaintext (readable, understandable data) and transforms it into ciphertext, a secure and unintelligible format. Once data is encrypted into ciphertext, the original plaintext becomes inaccessible until it is properly decrypted using the appropriate key. Now we will decrypt the file to view its content
<img width="2836" height="656" alt="image" src="https://github.com/user-attachments/assets/99b28ef2-53c2-4c2c-b1a8-96c58567eb22" />
This project demonstrates a practical implementation of symmetric encryption within an AWS environment using AWS KMS and the Encryption CLI. By securely creating and managing keys, configuring EC2 credentials, and executing encryption and decryption tasks, the solution establishes a foundational approach to protecting sensitive data in the cloud. The hands-on steps illustrate how plaintext is transformed into ciphertext and reliably decrypted, reinforcing key concepts of confidentiality and data lifecycle security using AWS-native services.
