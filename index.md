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
