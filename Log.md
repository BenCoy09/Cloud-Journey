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
# Day 3

## What I did
- Deepened my understanding of IaC through a back-and-forth Q&A challenge: config vs state file, terraform init vs apply, drift, why teams use version control for infrastructure
- Installed Terraform (v1.13.4) via HashiCorp's official source in WSL2/Ubuntu
- Learned what SSH is and why it's used to securely access remote cloud servers
- Launched a Linux EC2 instance on AWS
- Set up my .pem SSH key and moved it into my Ubuntu/WSL environment
- Used chmod 400 to set the correct permissions for my private key
- Found my EC2 public IPv4 address
- Connected to my EC2 instance using SSH from Ubuntu
- Verified I was inside the remote server

## What confused me
- Got "No such file or directory" because Ubuntu couldn't find my .pem file; wasn't sure if having the key on Windows instead of Ubuntu/WSL was the problem
- Got "Permission denied" after accepting SSH host verification, and learned that verifying the host and authenticating are separate steps
- Accidentally pasted part of the key into the terminal instead of the .pem filename, which gave "command not found"
- Learned I should reference the private key file with -i, not paste the key itself

## Tomorrow
- Practice more basic Linux commands on the EC2 server
- Continue with the next Learn to Cloud lesson
What I did

	•	Continued the Linux CTF challenges from Learn to Cloud
	•	Learned that /etc/resolv.conf is usually a symlink to a systemd-resolved file, and used resolvectl status to see the actual upstream DNS server vs the local stub resolver
	•	Learned scp has to run from my own machine, not the remote VM, since the destination is the VM
	•	Found that nginx doesn't have to run on the default port 80 — checked what it was actually listening on with ss -tlnp, then read its config to find the served directory
	•	Used tcpdump to capture live ICMP traffic and learned that ping packets can carry a hidden payload, visible in the ASCII column of a hex dump

What confused me

	•	I kept typing cd and cat on directories, forgetting that cat only works on files and ls is for directories
	•	I ran scp from inside my SSH session on the VM instead of my own laptop terminal, which is the opposite of how it needs to work

Tomorrow

	•	Continue with cron jobs, process inspection, and archive extraction challenges

Day 5

What I did

	•	Learned that scheduled tasks live in /etc/cron.d/, /etc/crontab, and per-user crontabs (crontab -l), and that a "do not edit" placeholder file is normal and unrelated to real jobs
	•	Learned that every running process has a folder under /proc/<PID>/, and its environment variables live in /proc/<PID>/environ as null-separated values, readable with tr '\0' '\n'
	•	Learned that short-lived commands like ps aux finish before you can inspect them, so I had to target a long-running process instead
	•	Practiced unpacking nested archives, going layer by layer with file to check the type before choosing tar -xzf or gunzip

What confused me

	•	I initially tried to cat a compressed archive directly, which just printed garbage, instead of extracting it first
	•	I didn't realize a PID has to be swapped in as a real number — I first ran the command with the literal word "PID" still in it

Tomorrow

	•	Continue with symlinks, bash history, and disk image mounting


	•	Forked the Linux CTFs repository to my own GitHub account and made sure it was public
	•	Submitted my completion token on learntocloud.guide
	•	Verified both Phase 1 requirements and completed Phase 1: Linux and Bash
	•	Reviewed my overall progress: Phase 0 (Starting from Zero) and Phase 1 (Linux and Bash) are both complete

What confused me

	•	My first verification attempt failed because the checker couldn't access the repo — I hadn't actually forked it yet, just typed in a URL

Tomorrow

	•	Start Phase 2: Networking Fundamentals
