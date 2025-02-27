## Defense in Depth

![7 Layers of Security](./assets/7-layers-security.png)
![CIA model](./assets/cia-model.png)

### Vulnerability

![Vulnerability Examples](./assets/Vulnerability.png)

---

### Encryption

- Encryption - Process of encoding information using a key and cipher to store sensitive data

  - Input: plain text; Output: ciphertext

- Cryptography - Practice and study of techniques for secure communication in the presence of third parties

- Cipher - An algorithm that performs encryption and decryption, also called a code

  - Output from encryption is called ciphertext

- Cryptographic Keys - A variable used in conjunction with an encryption algorithm

  - Two Types:
    1. Symmetric Encryption - Same key used for encryption and decryption
       - AES - Advanced Encryption Standard
    2. Asymmetric Encryption - Two keys used: one for encoding, one for decoding
       - RSA - Rivest-Shamir-Adleman

- Hashing - A function that accepts arbitrary size value and maps to fixed-size data structure

  - Reduces size of stored value
  - One-way process and deterministic (same output for same input)
  - Generally helpful in storing user passwords
  - Popular hashing algorithms: MD5, SHA256, Bcrypt

- Password Salting - Random string unknown to attacker that hash function accepts to mitigate deterministic nature of hashing function

- Digital Signature
  ![Digital Signature](./assets/digital-signature.png)

- Encryption Types

  1. Encryption in Transit - Secure when moving between locations
     - TLS, SSL
       1. TLS - 1.0 and 1.1 deprecated; 1.2 and 1.3 are best practice
       2. SSL - 1.0, 2.0, 3.0 deprecated

- Compliance Programs

  - Set of internal policies and procedures to comply with laws, rules, and regulations
    ![Compliance Program Ex 1](./assets/compliance-ex1.png)
    ![Compliance Program Ex 2](./assets/compliance-ex2.png)
    ![Compliance Program Ex 3](./assets/complinace-ex3.png)
    ![Compliance Program Ex 4](./assets/compliance-ex4.png)

- Security Testing

  - Penetration Testing - Authorized simulated cyberattack on computer system to evaluate security
  - DDoS testing exceptions:
    ![Pen Testing](./assets/pen-testing.png)

- AWS Security Services

  - AWS Artifact

    - Service portal to access AWS Compliance reports

  - AWS Inspector

    - Performs security checks against compute machines for virtual machine hardening
      ![AWS Inspector](./assets/inspector.png)

  - DDoS Protection

    - DDoS (Distributed Denial of Service) - Malicious attempt to disrupt normal traffic by flooding website
    - AWS Shield - Managed DDoS protection service
      - Automatic integration with Route 53 and CloudFront
      - Protects OSI model layers 3, 4, and 7
        ![AWS Shield Pricing](./assets/aws-shield-pricing.png)

  - AWS GuardDuty

    - Threat detection service that continuously monitors suspicious activities
    - Uses ML to analyze logs from CloudTrail, VPC Flow Logs, and DNS logs
    - Also known as IDS/IPS (Intrusion Detection/Prevention System)

  - AWS Macie

    - Fully managed service to monitor S3 data access activities
      ![AWS Macie](./assets/macie.png)

  - AWS VPN

    - Direct Connect provides private but not inherently secure connection
    - VPN provides both secure and private connection
      ![AWS VPN](./assets/vpn.png)

  - AWS WAF (Web Application Firewall)
    - Protects web applications from common attacks
    - Requires IP whitelist configuration in some cases
      ![AWS WAF](./assets/waf.png)

- Security Hardware

  - HSM (Hardware Security Module)

    - Hardware designed to store encryption keys in memory, never on disk
    - FIPS (Federal Information Processing Standard) Compliance:
      1. Multi-tenant HSM: FIPS 140-2 Level 2 compliant (AWS KMS)
      2. Single-tenant HSM: FIPS 140-2 Level 3 compliant (AWS CloudHSM)

  - AWS KMS (Key Management Service)
    ![KMS](./assets/kms.png)

  - AWS CloudHSM
    ![CloudHSM](./assets/CloudHSM.png)

- Security Initialisms
  ![Initialisms](./assets/Initialisms.png)

## Service Comparisons

- AWS Config vs AWS App Config
  ![AWS Config - AWS App Config](./assets/aws-config-vs-awsapp-config.png)

- SNS vs SQS
  ![SNS vs SQS](./assets/sns-sqs.png)

- SNS vs SES vs PinPoint vs WorkMail
  ![SNS vs SES vs PinPoint vs WorkMail](./assets/sns-ses-pinpoint-workmail.png)

- AWS Inspector vs AWS Trusted Advisor
  ![Inspector vs Trusted Advisor](./assets/inspector-vs-trusted-adviser.png)

- Connect Services
  ![Connect Service](./assets/connect-services.png)

- Elastic Transcoder vs MediaConvert

  - Elastic Transcoder is legacy service
    ![Elastic Transcoder vs MediaConvert](./assets/elastic-transcoder-vs-media-converter.png)

- AWS Artifact vs Amazon Inspector
  ![Artifact vs Inspector](./assets/artifacts-vs-inspector.png)

- AWS ELB Types
  - Network Load Balancer (NLB) recommended for gaming applications
    ![ELB](./assets/elb-types.png)
