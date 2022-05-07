# Welcome to the DevOps Homelab Setup Guide

For starters, a homelab is a 'playground' for IT professionals, developers, and just about anyone to grow their technical skills in a non production environment. My primary background is that of a DevOps engineer, with a heavy emphasis on the Operations side of things.

You don't have to learn everything that's covered in this guide, or everything covered in the [incredible roadmap found here](https://roadmap.sh/devops). However, even a little bit of additional training goes a long way! 

---
## Cloud

The 'cloud' is one of the biggest buzzwords in tech at the moment and you would do well to dip your toes into it! Luckily, this is one of the easiest and cheapest things to learn at the moment thanks to how heavily some companies are pushing their cloud infrastructures.

### AWS

I know I'm listing this first, but it actually isn't my favorite cloud provider for beginners anymore. However, they are undoubtedly the market leaders at the moment, so their certifications are king in the space. 

Luckily, they provide 100% free training for their entry level certification 'AWS Cloud Practitioner'. The training can be [found here](https://aws.amazon.com/training/digital/aws-cloud-practitioner-essentials), and it's estimated to only take around 6hrs to complete and prepare for the exam. Once you've knocked that out, it will also earn you a 50% off voucher for any AWS certification exam you take after that!

For actually training your skills, [these are all the services you can deploy for free within AWS](https://aws.amazon.com/free/). However, I personally find their offerings rather weak as at most you're getting 1 reliably free VM for playing around. 

### Oracle Cloud

Last I checked, they don't even hold 5% of the overall Cloud Market share, and that's exactly why they're perfect for homelabs! You get around 6x the compute with the [Oracle Cloud Free Tier](https://www.oracle.com/cloud/free/) than you would with AWS. For your first 30 days, you also get $300 in free credits to explore services that aren't covered in the free tier and this could be your chance to learn your way around Kubernetes at no cost to you!

They've also got a bunch of [free learning resources that can checked out here](https://education.oracle.com/learning-explorer#startLearning). However, I'm not entirely sure how strong their certifications are in the market at this time. You'll come to realize soon though, that despite naming their services a little bit differently than AWS, the core concept behind the both is the same, and so they'll both benefit you greatly.

---
## Linux
Different flavors of Linux rule the compute market in the cloud, so it would be wise to learn it!
Luckily, you've signed up for either AWS or Oracle Cloud by now and have access to 1 or 6 Linux VMs now. My favorite distros to learn and play around with are.
- Debian
- Oracle Linux
- Red Hat
- Ubuntu
- Amazon Linux

Redhat undeniably rules the enterprise Linux market right now, so it would be very wise to learn it. Luckily, individuals can get [access to Red Hat for free via this link](https://developers.redhat.com/products). The rest of the operating systems are free, and Oracle Linux is 100% free while building on top of Red Hat so its perfect if you prefer an easier route without having to deal with Red Hat licensing. 

---

## Selfhosting

So you've got multiple servers all hosted within the cloud at this point with public IP's, what do you do with them?
Start selfhosting applications of course!
This will teach you more about how websites or applications work on the backend which in production environments is what we are dedicated to supporting. 

[This just happens to be a link to a wonderful Github repo that has listed out various network services and web applications which can be hosted on your own servers](https://github.com/awesome-selfhosted/awesome-selfhosted).
More interested in the SysAdmin side of things? Wondering how companies host their own VPN servers?
Well [here is a list of awesome open source sysadmin resources that you can once again host on your servers](https://github.com/kahun/awesome-sysadmin).

---

## Bare Metal vs Containerized Applications

If you've started selfhosting, you may naturally turn to installing applications directly onto the host. However, I think you'll find that occasionally you'll run into issues when multiple applications have conflicting dependencies or it'll get annoying separating your apps across multiple VMs to avoid these issues. 

A lot of the applications from the selfhosting repo have instructions for installing them within Docker. I urge you to explore that option, and [watch this video that explains the difference between both architectures](https://www.youtube.com/watch?v=XCWWPpfdbsM) better than I. 

---

## First App?

I recommend everyone start with [littlelink](https://github.com/sethcottle/littlelink) for their first deployment. If you follow that link it'll take you to their Github repo, and there's a one click deploy button from there. You'll have to sign up for Github, but trust me you'll wanna do that anyway. 

Littlelink is essentially a git controlled dashboard that you can use to link to your other websites. It'll be hosted by Vercel for free as it falls under 'non-commercial & hobby sites' and they handle a lot behind the scenes to make it easier to learn this stuff little by little. This dashboard will be great to have once you've got other hosted projects, as it makes for the perfect landing page that you can link to on your resume to show employers or friends the projects you've been working on.

---

## Git

Don't think you can skip this section, I know you've got a Github account now if you followed the section above. [Watch this 20 minute video explaining Git, Github, and Github Desktop](https://www.youtube.com/watch?v=8Dd7KRpKeaE) (Simplified Git).
Trust me, git repositories work perfectly with a lot of automation tools that will be covered later on. 

---

## YAML

YAML is the language used by multiple Infrastructure as Code tools, so [here is a video covering its structure](https://www.youtube.com/watch?v=1uFVr15xDGg). [This is a guide from Google on what Infrastructure as code, and it includes an example of a basic configuration file that is utilizing YAML](https://www.youtube.com/watch?v=z-caqPtEw58).

---

## Terraform

You should definitely learn to build, change, and destroy infrastructure with Terraform. If you've experimented with bringing up virtual machines, you'll quickly realize how tedious the whole process can be, not to mention having to bring up a virtual network for your VM to live in.

On their website, they have [free learning lessons](https://learn.hashicorp.com/terraform). The cool thing is, once you learn Terraform with any infrastructure provider, whether it be AWS, Oracle Cloud, or Docker, the skills you learn will be easily transferrable to other infrastructure providers. Terraform is a tool for 'Infrastructure as Code', but please don't be intimidated, as once you get started with the tutorials, you'll realize no coding language experience is required. Here is a cool video that explains and compares Terraform and Ansible in just 15 minutes.

---

## Ansible

Another tool in the world of 'Infrastructure as Code', but with a heavier focus on the configuration aspect of equipment. This is a [great video on real world automation with Ansible](https://www.youtube.com/watch?v=w9eCU4bGgjQ&t=445s). However, while I believe this is the nicest tutorial I've seen, it covers the CLI version of Ansible, and it's important to note that there is a graphical version of Ansible known as Ansible Tower. There are free versions of this graphical Ansible manager, such as AWX Tower or Oracle Automation Manager. I highly recommend using one of your Oracle Cloud VMs to deploy their version of this [Automation Manager using this tutorial](https://docs.oracle.com/en/operating-systems/oracle-linux/8/oracle-linux-automation-manager/awx-AboutOracleLinuxAutomationManagerandOracleLinuxAutomationEngine.html#awx-about).