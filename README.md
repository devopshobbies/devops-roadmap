# DevOps-Roadmap

<p align="center">
 <img alt="DevOps-Logo" src="image/DevOps.png">
</p>

## Introduction
📌 DevOps is a set of practices that combines software development and IT operations. It aims to shorten the systems development life cycle and provide continuous delivery with high software quality. DevOps is complementary with Agile software development; several DevOps aspects came from the Agile methodology.

### Table of Contents

- [Programing Language](#programing-language)
  - [Python](#Python)
  - [Golang](#Golang)
- [DevOps Overview](#devops-overview) 
- [Step 0: Basic requirements](#step-0-basic-requirements)
  - [Linux (LPIC-1)](#linux-lpic-1)
  - [Docker (Mandatory)](#docker-mandatory)
  - [Containers From Scratch (Optional)](#Containers-from-scratch-optional)
  - [Containerd or LXC (Optional)](#containerd-or-lxc-optional)
  - [Bash-Script](#bash-script)
  - [Git](#git)
  - [NetOps](#netops)
- [Step 1: IaC (Infrastructure as Code)](#step-1-iac-infrastructure-as-code)
  - [Hashicorp Terraform (Strongly Recommended)](#hashicorp-terraform-strongly-recommended)
  - [Pulumi (Normal)](#pulumi-normal)
- [Step 2: Configuration Managment](#step-2-configuration-managment)
  - [Ansible (Strongly Recommended)](#ansible-strongly-recommended)
  - [Puppet (Important)](#puppet-important)
  - [SaltStack (Normal)](#saltstack-normal)
  - [Chef (Normal)](#chef-normal)
- [Step 2.5: End-to-End Automation](#step-25-end-to-end-automation)
  - [End-to-End Automation on VMware vsphere with Ansible and Terraform](#end-to-end-automation-on-vmware-vsphere-with-ansible-and-terraform)
  - [Build all instance images with Hashicorp Packer](#build-all-instance-images-with-hashicorp-packer)
- [Step 3: CI/CD (Continuous Integration and Continuous Delivery)](#step-3-cicd-continuous-integration-and-continuous-delivery)
  - [Jenkins (Suitable for CI and CD in ALL infrastructure)(Free) (Strongly Recommended)](#jenkins-suitable-for-ci-and-cd-in-all-infrastructurefree-strongly-recommended)
  - [GitLab (Suitable for CI and CD in ALL infrastructure)(Paid)](#gitlab-suitable-for-ci-and-cd-in-all-infrastructurepaid)
  - [GitHub (GitHub Actions)(Paid)](#github-github-actions-free)
  - [Azure DevOps (Suitable for CI and CD in Windows infrastructure)(Paid)](#azure-devops-suitable-for-ci-and-cd-in-windows-infrastructurepaid)
  - [CircleCI (Paid)(Important)](#circleci-paidimportant)
  - [Teamcity (Paid)](#teamcity-paid)
  - [Bamboo (Paid)](#bamboo-paid)
- [DevOps Projects](#devops-projects)
- [Step 3.1: Object Storage](#step-31-object-storage)
  - [MiniO](#minio)  
- [Step 4: Container Orchestration](#step-4-container-orchestration)
  - [Kubernetes](#kubernetes)
  - [Helm (Kubernetes Package manager)](#helm-kubernetes-package-manager)
- [Step 4.5: GitOps Implementation](#step-45-gitops-implementation)
  - [Jenkins-X (CI/CD) (Free)](#gitops)
  - [ArgoCD (CD) (free)](#gitops)
  - [Spinnaker (CD) (free)](#gitops)
  - [Helm (Kubernetes Package manager)](#helm-kubernetes-package-manager)
- [Step 5: Monitoring and Logging](#step-5-monitoring-and-logging)
  - [Prometheous + Grafana (Free)](#prometheous--grafana-free)
  - [Grafana LGTM Stack (Loki + Grafana + Tempo + Mimir) (Free)](#grafana-lgtm-stack-loki--grafana--tempo--mimir)
  - [Zabbix + Grafana (Free)](#zabbix--grafana-free)
  - [Telegraf + InfluxDB + Grafana (Free)](#telegraf--influxdb--grafana-free)
  - [Datadog (Paid)](#datadog-paid)
  - [ELK Stack (Free)](#elk-stack-free)
  - [NewRelic (Paid)](#newrelic-paid)
- [Step 6: Public Clouds](#step-6-public-clouds)
  - [Amazon Web Services (AWS)](#amazon-web-services-aws)
  - [Microsoft Cloud (Azure)](#build-all-instance-images-with-hashicorp-packer)
  - [Google Cloud (GCP)](#build-all-instance-images-with-hashicorp-packer)
- [DevOps Projects](#devops-projects-1)
- [Step 7: Getting familiar with Agile software development](#step-7-getting-familiar-with-agile-software-development)
- [Contact the maintainer of DevOps Hobbies](#maintainer)


## Programing Language
📌 Consider this as your benefit. A good DevOps engineer know at least one popular programming language.

- ### Python
  - Videos:
    - [Python Learning with Jadi on Youtube](https://www.youtube.com/watch?v=BR7m_2D_-Uw&list=PL-tKrPVkKKE1Y_o_h2w85dzVdoX5t7SI0) (Persian Language) (Free)
    - [Python Learning with Jadi on Aparat](https://www.aparat.com/v/Fk27n) (Persian Language) (Free)
    - [Learn Python at the elementary and intermediate level](https://toplearn.com/courses/2150/%D8%A2%D9%85%D9%88%D8%B2%D8%B4-%D8%B1%D8%A7%DB%8C%DA%AF%D8%A7%D9%86-%D9%BE%D8%A7%DB%8C%D8%AA%D9%88%D9%86-(-python-)) (Persian Language videos) (Free)
    - [Python Zero to Hero - Andrei Neagoie](https://www.youtube.com/playlist?list=PL3JcF91tUKYYIbjAAZ2Y8UNp2IhqEAFSW) (English Language) (Free)
  - Books/Docs/Code:
    - [Learn Python 3 the Hard Way](https://www.amazon.com/Learn-Python-Hard-Way-Introduction/dp/0134692888/ref=sr_1_1) (Includes projects to apply the knowledge)
    - [Effective Python: 90 Specific Ways to Write Better Python](https://www.amazon.com/Effective-Python-Specific-Software-Development/dp/0134853989/ref=sr_1_1) (Explains the Python best practices by using sample codes in different situations)
- ### Golang
  - Videos:
    - [Go Master Class - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=3GIEmRfMA0I&list=PLYrn63eEqAzYOwqstIZWW4Q8dQ3Ncchbw&pp=iAQB) (Persian Language) (Free)
    - [Golang Tutorial for Beginners](https://m.youtube.com/watch?v=YS4e4q9oBaU) (English Language) (Free)
  - Books/Docs/Code:
    - [Practical Go Lessons](https://www.practical-go-lessons.com/) (English book for beginners)
    - [Golang Tutorial](https://gobyexample.com/) (English book for beginners)
## DevOps Overview
  - Videos:
    - [DevOps Overview -  Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=M8ztRU94XNg&list=PLYrn63eEqAzbtAEHtmbhxxrwCCNYrRUDv) (Persian Language) (Free)
## Step 0: Basic requirements
- ### Linux (LPIC-1)
  - Videos:
    - [LPIC-1: Linux Administrator (101-500 and 102-500)](https://app.pluralsight.com/paths/certificate/lpic-one) (You need to have pluralsight subscribtion to see this courses. This path is around 30 hours and it's so amazing) (English Language)
    - [OLD LPIC-1 Learning with Jadi](https://www.aparat.com/v/vw7Gl?playlist=207575) (Persian Language)
    - [New LPIC-1 Learning with Jadi (Recording)](https://www.youtube.com/watch?v=cqfrsmg4BKo&list=PL-tKrPVkKKE0kM18Sg5fqaZW1V2nidAeU&index=1) (Persian Language)
    - [New LPIC-1 Learning with Jadi (Recording)](https://www.youtube.com/watch?v=AKkNUvEHXhk&list=PLFOYXCPEqdNUU55Xvgst8wGTWnz_sd-cj) (English Language)
    - [Jadi's free LPIC 1 book](https://linux1st.com/) (English Language)
    
- ### Docker (Mandatory)
  - Videos:
    - [Docker for the Absolute Beginner](https://kodekloud.com/courses/docker-for-the-absolute-beginner/) (This course is free and it's a good start for learning docker)
  - Books/Docs/Code:
    - [Docker Deep Dive By  Nigel Poulton](https://www.amazon.com/Docker-Deep-Dive-Nigel-Poulton/dp/1521822808/ref=tmm_pap_swatch_0) (English book for beginners to have a fundamental knowledge of how to use Docker)
- ### Containers From Scratch (Optional)
  - Videos:
    - [Containers From Scratch - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=pC6utshJRW8&list=PLYrn63eEqAzbB6IpUB7BFDcDbuPvvnERl) (Persian Language) (Free)
- ### Containerd or LXC (Optional)
  - Videos:
    - [Containerd Deep Dive](https://www.youtube.com/watch?v=UUDDCetB7_A)


- ### Bash-Script
  - Videos:
    - [Bash Script Learning - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=b92kh67V4Mw&list=PLYrn63eEqAzYb9UoaaLJD1fdtoPx5jpaG) (Persian Language videos) (Free)
    - [Bash Script Tutorial With Alireza Amirsamimi](https://amirsamimi.ir/bash_tutorials/) (Persian Language videos) (Free)
  - Books/Docs/Code:
    - [Bash Script Tutorial](https://github.com/ahmadalibagheri/bash-script-tutorial) (Sample Traning Code)
    - [Linux Command Line and Shell Scripting Bible 4th Edition](https://www.amazon.com/Linux-Command-Shell-Scripting-Bible/dp/1119700914/ref=pd_bxgy_img_sccl_2/145-7066057-4592848) (LPIC1-Level English book including shell scripting as well as Linux concepts)
    
- ### Git
  - Videos:
    - [Git Learning with Jadi](https://faradars.org/courses/fvgit9609-git-github-gitlab) (Persian Language) (Free)
    - [Git Learning with Roocket](https://roocket.ir/series/learn-git-and-github) (Persian Language) (Free) 
    - [Git Learning with Mosh](https://codewithmosh.com/p/the-ultimate-git-course) (English Language) (Free)
  - Books/Docs/Code:
    - [Ry's Git Tutorial](https://www.amazon.com/Rys-Git-Tutorial-Ryan-Hodson-ebook/dp/B00QFIA5OC/ref=sr_1_15) (English book for all grades)
  - Games:
    - [Oh my git!](https://ohmygit.org/) (English Language)(If you prefer to learn while having fun)
- ### NetOps
  - Videos:
    - [NetOps - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=zRizf-tRln4&list=PLYrn63eEqAzaydfpPB9tTFVTUTkneP6EN) (Persian Language) (Free)

## Step 1: IaC (Infrastructure as Code)
- ### Hashicorp Terraform (Strongly Recommended)
  - Videos:
    - [Terraform From Zero to Hero - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=aFk04rQWvOM&list=PLYrn63eEqAzZssgLu8Um_k1v8Pvh7-l7b) (Persian Language) (Free)
    - [Terraform Tutorial by Hamed Farvardin](https://linux.tosinso.com/fa/videos/10492/%D8%A2%D9%85%D9%88%D8%B2%D8%B4-%D8%AA%D8%B1%D8%A7%D9%81%D8%B1%D9%85-(Terraform)-%D9%82%D8%B3%D9%85%D8%AA-1-%D9%85%D8%B9%D8%B1%D9%81%DB%8C-%D8%AA%D8%B1%D8%A7%D9%81%D9%88%D8%B1%D9%85) (Persian Language) (Paid)
  - Books/Docs/Code:
    - [Terraform Tutorial](https://github.com/ahmadalibagheri/terraform-tutorial) (Sample Traning Code from non public cloud provider)
    - [Getting Started With Terraform on AWS by Sumeet Ninawe](https://spacelift.io/blog/terraform-tutorial) (Terraform Tutorial )
- ### Pulumi (Normal)

## Step 2: Configuration Managment
- ### Ansible (Strongly Recommended)
  - Videos:
    - [Getting Start With Ansible](https://www.youtube.com/watch?v=3RiVKs8GHYQ&list=PLT98CRl2KxKEUHie1m24-wkyHpEsa4Y70) (Beginner Video)
    - [Ansible with Morteza Bashsiz](https://www.youtube.com/playlist?list=PLRMCwJJwWR1AKYcUkdcorTFR-bhXUN6oO) (Persian Language) (Free) (Beginner Video)
  - Books/Docs/Code:
    - [Ansible Tutorial](https://github.com/ahmadalibagheri/Ansible-tutorial) (Sample Traning Code)
    - [Ansible: From Beginner to Pro](https://www.amazon.com/Ansible-Beginner-Pro-Michael-Heap/dp/1484216601/ref=sr_1_19) (Beginner Book)
    - [Ansible for DevOps](https://www.amazon.com/Ansible-DevOps-Server-configuration-management/dp/0986393428/ref=sr_1_4) (Advanced Book)
- ### Puppet (Important)
- ### SaltStack (Normal)
  - Videos:
    - [Learning SaltStack](https://www.youtube.com/playlist?list=PLgGQIE0cGrkiDRmJ3YWBKlI2KuYfFvfzV) (English Language) (Free)
- ### Chef (Normal)

### Step 2.5: End-to-End Automation
on this step you need to learning End-to-End automation with Ansible and Terraform on infrastruture. Please follow bottom repos.
- #### End-to-End Automation on VMware vsphere with Ansible and Terraform
  - Books/Docs/Code:
    - [Terraform vsphere Ansible Tutorial](https://github.com/ahmadalibagheri/terraform-vsphere-ansible) (Sample Training Code)
- #### Build all instance images with Hashicorp Packer
  - Videos:
    - [Packer Tutorial For Beginners](https://www.youtube.com/watch?v=tbv1lTF1wFU&list=PL8VzFQ8k4U1Jp6eWgHSXHiiRWRvPyCKRj&index=1) (English Language) (Free)
  - Books/Docs/Code:
    - [Packer Tutorial](https://github.com/ahmadalibagheri/packer-tutorial)

## Step 3: CI/CD (Continuous Integration and Continuous Delivery)
- ### Jenkins (Suitable for CI and CD in ALl infrastructure)(Free) (Strongly Recommended)
  - Videos:
    - [Jenkins CICD - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=l9XXgAHNM4M&list=PLYrn63eEqAzaErni2aBsPEhKhoxiX7yes) (Persian Language) (Free)
- ### GitLab (Suitable for CI and CD in ALl infrastructure)(Paid)
  - Videos:
    - [Gitlab CICD - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=M0OWvEE4e3I&list=PLYrn63eEqAzannVocQrddqsBK-C17e-Sm) (Persian Language) (Free)
  - Books/Docs/Code:
    - [Mastering GitLab 12: Implement DevOps culture and repository management solutions](https://www.amazon.com/Mastering-GitLab-Implement-repository-management-ebook/dp/B07W6F6SGG/ref=sr_1_3) (Beginner-To-Advanced English book to get familiar with GitLab and its scenarios as the real-world examples explain.)
- ### GitHub (GitHub Actions) (Free)
  - Videos:
    - [Automate your workflow from idea to production](https://youtu.be/X3F3El_yvFg) (CI/CD With GitHub Actions) (English Language) (Free)
- ### Azure DevOps (Suitable for CI and CD in Windows infrastructure)(Paid)
  - Videos:
    - [AzureDevOps + CI/CD + .netcore - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=lBjX9PXEvEw&list=PLYrn63eEqAzZGQMqdZDDgdqud0FrvNzNp) (Persian Language) (Free)
- ### CircleCI (Paid)(Important)
- ### Teamcity (Paid)
- ### Bamboo (Paid)

## DevOps Projects
  - Videos:
    - [Django + Docker + CI/CD - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=KtYDIJN3wmM&list=PLYrn63eEqAzY5uG5ks_OquWcojzHvhp9Z) (Persian Language) (Free)

## Step 3.1: Object Storage
- ### MiniO
  - Videos:
    - [MiniO Tutorial - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=y4of6U-mdVQ&list=PLYrn63eEqAzaS7mHcJh7GPOFWcLHLxlfE) (Persian Language) (Free)   

## Step 4: Container Orchestration
- ### Kubernetes
  - Videos:
    - [Kubernetes Tutorial for Beginners [FULL COURSE in 4 Hours]](https://www.youtube.com/watch?v=X48VuDVv0do) (It's a great start to learn what is kubernetes)(Free)
    - [Certified Kubernetes Administrator (CKA)](https://www.udemy.com/course/certified-kubernetes-administrator-with-practice-tests/) (Kubernetes Administration course by Mumshad, also has a free lab on kodekloud for anyone who bought the course from udemy)(Paid)
  - Books/Docs/Code:
    - [Kubernetes Complete Reference](https://github.com/ahmadalibagheri/kubernetes-complete-reference) (Sample Traning Code)
  - Real-World sample code
    - [Kubernetes in real world](https://github.com/Mozart4242/kubernetes-real-world)

- ### Helm (Kubernetes Package manager)
  - Videos:
    - [Learn Helm with this full "Mini Course" - Richard Chesterwood](https://www.youtube.com/playlist?list=PLSwo-wAGP1b8svO5fbAr7ko2Buz6GuH1g) (English Language) (Free)

### Step 4.5: GitOps Implementation
- #### GitOps
  - Videos:
    - [Argo From Zero To Hero - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=T-ERIOb_3z0&list=PLYrn63eEqAzYttcyB6On1oH35O5rxgDt4) (English Language) (Free)
  - Books/Docs/Code:
    - [Jenkins-X](https://jenkins-x.io/) (CI/CD) (Free)
    - [ArgoCD](https://argo-cd.readthedocs.io/en/stable/) (CD) (free)
    - [Spinnaker](https://spinnaker.io/) (CD) (free)

## Step 5: Monitoring and Logging
- ### Prometheous + Grafana (Free)
  - Books/Docs/Code:
    - [Prometheus: Up & Running: Infrastructure and Application Performance Monitoring](https://www.amazon.com/Prometheus-Infrastructure-Application-Performance-Monitoring/dp/1492034142/ref=sr_1_1) (English Book)
  - Videos:
    - [Prometheus Tutorial | Monitoring with Prometheus And Grafana | Prometheus Grafana Tutorial | Edureka](https://www.youtube.com/watch?v=7gW5pSM6dlU)
- ### Grafana LGTM Stack (Loki + Grafana + Tempo + Mimir)
  - Videos:
    - [Grafana LGTM Stack - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=boS5enCeszU&list=PLYrn63eEqAzZL2TaS0pXXw-_DEl3SsAF_) (English Language) (Free)
- ### Zabbix + Grafana (Free)
  - Videos:
    - [Zabbix And Grafana - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=s4CuvB5-NZE&list=PLYrn63eEqAzaEkGmYAn6StHk4rqVEjd_g) (Persian Language) (Free)
- ### Telegraf + InfluxDB + Grafana (Free)
- ### Datadog (Paid)
- ### ELK Stack (Free)
  - Videos:
    - [Complete Guide to Elasticsearch](https://www.udemy.com/course/elasticsearch-complete-guide/) (To learn elasticsearch itself)
    - [Data Visualization with Kibana](https://www.udemy.com/course/data-visualization-with-kibana/) (To learn the visualizations with Kibana)
    - [Data Processing with Logstash and Filebeat](https://www.udemy.com/course/processing-events-with-logstash/) (To learn the pipeline design and implementation using Logstash)
- ### NewRelic (Paid)
  - Books/Docs/Code:
    - [Newrelic University](https://learn.newrelic.com/)
  - Videos:
    - [APM Certification Training](https://www.youtube.com/watch?v=uf1WrQsfhy8)
- ### EFK Stack (Free)

## Step 6: Public Clouds
- ### Amazon Web Services (AWS)
  - Video:
     - [AWS Certified Cloud Practitioner](https://www.itpro.tv/courses/aws/aws-certified-cloud-practitioner/) (Paid)
     - [AWS Certified DevOps Engineer - Professional](https://www.itpro.tv/courses/aws/aws-certified-devops-engineer-professional-dopc01/) (Paid)
## DevOps Projects
  - Videos:
     - [AWS + Cloudflare + Vercel - Created by the DevOps Hobbies Team](https://www.youtube.com/watch?v=SqE6spnJ6LE&list=PLYrn63eEqAzYnojn7knFSiQgir2qjVMQ9) (Persian Language) (Free)

## Step 7: Getting familiar with Agile software development
📌 If you made yourself through here, it means that you are now a capable DevOps Engineer. from now on, we need to focus on something furthur than using technologies. in order to become a senior, you need to be aware of all the aspects.


- [Agile Software Development](https://en.wikipedia.org/wiki/Agile_software_development)
- [Agile Software Development, Principles, Patterns, and Practices](https://www.amazon.com/Software-Development-Principles-Patterns-Practices-ebook/dp/B00IZ0G6YG)


## Maintainer
  - Ahmadali Bagheri
    - [Email](Ahmad@devopshobbies.com)
    - [Github](https://github.com/ahmadalibagheri)
    - [LinkedIn](https://www.linkedin.com/in/ahmadali-bagheri/)
