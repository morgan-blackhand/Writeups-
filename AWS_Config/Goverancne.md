# AWS Config: Managing Encryption and Tags for Compliance

## Introduction
This document outlines the process of using AWS Config to enforce server-side encryption on S3 buckets and manage resource tagging, ensuring compliance across AWS services.

## Steps
1. **Setting Up AWS Config for S3 Encryption:**
   - Begin by creating a rule in AWS Config that mandates encryption on S3 buckets. This involves setting up server-side encryption with AWS Key Management Service (KMS).

(https://imgur.com/a/roc1HgH)
https://imgur.com/a/0Pu8g3C


2. **Compliance Dashboard Review:**
   - Navigate to the AWS Config dashboard to monitor for any compliance issues related to the new encryption rule.
  
     https://imgur.com/a/xImfWjG

3. **Addressing Compliance Issues:**
   - If any issues are detected, adjust the default encryption settings by integrating server-side encryption with KMS to resolve these issues.


(https://imgur.com/a/R7PQJxc)

https://imgur.com/a/jlffSk4

4. **Tagging Rule Configuration:**
   - Implement a rule requiring tags on your AWS resources. Initially, this applies to all resources but is later adjusted to specifically target only EC2 instances.

https://imgur.com/a/xFIAiWP

5. **Resource Tagging:**
   - Proceed to tag EC2 resources as required by the newly configured rule.

https://imgur.com/a/GMsAik8

6. **Saving and Reviewing Configurations:**
   - After tagging, save the configurations and review the AWS Config screen to ensure all changes are correctly implemented.


https://imgur.com/a/yS2JQb4

7. **Compliance Reevaluation:**
   - Finally, add at least one required tag to your EC2 instance to simplify the process. Then, reevaluate the compliance rules to confirm if your setup meets all required configurations.

https://imgur.com/a/J5TRhqB

## Conclusion
This lab illustrates the utilization of AWS Config to enforce essential security and compliance measures such as encryption and tagging within AWS environments. Regular monitoring and updating of these configurations ensure adherence to best practices and organizational policies.

## Reflection
- The ability to swiftly rectify compliance issues and update configurations highlights the dynamic capabilities of AWS Config, crucial for maintaining an efficient and secure cloud infrastructure.

