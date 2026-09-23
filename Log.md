# Day 1

## What I did
- Set up my GitHub profile (bio, links) and created this repo
- Updated my LinkedIn and added my GitHub link
- Started Learn to Cloud, Phase 0: Starting from Zero
- Learned why cloud companies use Linux: stable, controllable from the command line, cheap (no license fees), and containers rely on it
- Learned Bash basics: terminal vs shell vs Bash, and what a command, option and argument are
- Learned that cp copies a file and mv moves or renames it

## What confused me

- I wondered why "ls" appeared twice. It was the same command, once as an example to explain the parts of a command and once as a command to learn.

- I worried about memorizing all the commands. I learned that I can practice a few at a time and look up the rest.


## Tomorrow
- Star the Learn to Cloud repo, install VS Code, and install WSL2
- Practice pwd, ls, cd, mkdir and cat in the terminal
# Day 2

## What I did
- Fixed a PowerShell (x86) issue and installed WSL2 with Ubuntu
- Practiced pwd, ls, cd, mkdir, touch, and cat in the Linux terminal
- Learned networking fundamentals: IP addresses (public/private), DNS, ports, and SSH
- Installed Python (already had 3.14.4) and wrote a script that parses JSON data
- Learned DevOps fundamentals: version control, Infrastructure as Code, CI/CD, observability, containers, and Kubernetes
- Learned cloud computing basics (IaaS/PaaS/SaaS) and chose AWS as my main cloud provider
- Created an AWS Free Tier account, verified my card, and set up a zero-spend billing alert
- Fixed a failed GitHub profile README verification and completed all of Phase 0

## What confused me
- I mixed up domain names, IP addresses, and DNS at first, but got it clear: an IP is the number, a domain is the human-friendly name, and DNS is the phonebook that connects them
- I wasn't sure why SSH and RDP don't need their own domains, but learned one domain can serve any port or protocol

## Tomorrow
- Start Phase 1: Linux and Bash properly
Day 3

What I did

* Started Learn to Cloud, Phase 1: Cloud
* Started the Cloud CLI section and chose AWS as my cloud provider
* Installed the AWS CLI on my Linux/Ubuntu environment
* Verified the installation with aws --version
* Learned that the AWS CLI lets me interact with AWS services directly from the terminal
* Created an IAM user for my CLI access
* Created AWS access keys for the IAM user
* Configured the AWS CLI with aws configure
* Set my default AWS region to us-east-1
* Set the default output format to json
* Verified that my AWS credentials were working with aws sts get-caller-identity
* Successfully completed the Cloud CLI authentication setup

What confused me

* I wasn’t sure where the AWS Access Key ID and Secret Access Key came from. I learned that they are created through an IAM user’s security credentials.
* I initially entered one of the configuration values incorrectly and had to correct it.
* I wasn’t sure what to put for the default region and output format. I learned that the region determines where AWS resources are created/managed, while json controls how CLI output is displayed.
* I learned that installing the AWS CLI and authenticating it are two separate steps.

Tomorrow

* Continue with Phase 1: Cloud
* Learn more AWS CLI commands
* Start working with AWS services from the terminal
* Keep practicing Linux/Bash alongside the cloud labs
