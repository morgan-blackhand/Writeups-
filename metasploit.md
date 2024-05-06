# Google Cloud VM Writeup

## Metasploit Setup

We start by working on Metasploit and doing `netdiscover` to find the IP of Metasploit. Then, we open `msfconsole` and search for the `vsftpd` exploit that's used to exploit port 21. Since it's not in the photo, set your payload to `set PAYLOAD cmd/unix/reverse_perl`.

https://imgur.com/a/EEwWVHb

Once you select your payload, set your local host for `lhosts` and `rhosts` for the target. Once you set your payload and hosts, type `exploit` and then type `id` to verify if you're in.

https://imgur.com/a/TSMlDNc

## SMB Exploit

Now that we've done that, let's try to get in through SMB using an exploit. You just need to go through choosing the correct SMB, then set your host, and run `exploit`. Once you run the exploit, try to log into SMB and you should be in.

https://imgur.com/a/XI1AfWm
https://imgur.com/a/Xnfr5Bt

These are the main two ways to use Metasploit to exploit Metasploitable 2.



## Google Cloud VM Setup

I went through a lot of experimenting and trying different ways to do this and make it more advanced. I made a VM online in Google Cloud, and I was able to transfer over VMDK and look at the logs. However, even after adding the needed ingress and egress rules, I wasn't able to exploit anything. 

Here are the steps and link with photos: https://imgur.com/a/87vmHfV

# Virtual Machine Disk Conversion and Deployment Process

### Step 1: Convert VMDK to "disk.raw"
> **Note:** This process is not pictured.
- **Task**: Convert a VMDK file to a disk image named "disk.raw" which is required for further steps.

### Step 2: Compress the Disk into `target.tar.gz`
> **Command**:
```bash
tar -czvf target.tar.gz disk.raw

    Note: Here's the command used to compress the disk into a .tar.gz file.

Step 3: Upload the Compressed File to a Bucket

    Command:

bash

gsutil cp target.tar.gz gs://your-bucket/

    Note: The process of uploading using this command is not pictured.

Step 4: Create the Virtual Machine with the Disk

    Task: Use the compressed disk file to create and configure the virtual machine.

Step 5: Nmap Scan the Target

    Note: This step is not pictured.

    Task: Perform an Nmap scan on the target to evaluate network security and open ports.

Step 6: Activate the Flow Logs

    Task: Enable flow logs to monitor and record network traffic associated with the virtual machine.

Step 7: Analyze the Flow Logs with AI

    Task: Use AI tools to analyze and format the flow logs into a more understandable representation.

vbnet


This Markdown document provides a detailed step-by-step guide for each part of your process
