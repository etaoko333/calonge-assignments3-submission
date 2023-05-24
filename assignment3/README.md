## Kubernetes, Docker, Containerisation and Virtualisation

1. What is a hypervisor and where does it sit in the server virtualisation stack?
ans: A hypervisor is a layer of software that enables multiple virtual machines (VMs) to run on a single physical server. It manages the allocation of resources, such as CPU, memory, and storage, among the virtualized instances. Hypervisors also provide isolation between VMs and between VMs and the host operating system.

Hypervisors sit at the lowest level of the server virtualization stack. Above the hypervisor are the virtual machines themselves, each running its own operating system, applications, and services. The hypervisor provides the interface between the physical server's hardware and the virtualized instances, allowing each VM to access the resources it needs to operate.



2. What is a container runtime and name the two most common runtimes? ans: A container runtime is a software component that enables the creation and management of containers, which are lightweight, portable, and isolated environments that isolate an application and its dependencies. The container runtime is responsible for launching containers and ensuring that they have the necessary resources to run.

The two most common container runtimes are:

1. Docker: Docker is a popular container runtime that provides a user-friendly interface for creating, managing, and running containers. It simplifies the process of building and deploying applications in containerized environments. Docker uses a client-server architecture and can run on various platforms, making it a versatile choice for containerization.

2. Container: Containerd is an open-source container runtime that provides low-level container management functionality. It is designed to be lean and efficient, providing a foundation for higher-level container orchestration platforms like Kubernetes. Containerd can also support multiple image formats and storage backends, making it a flexible choice for containerization.


## Linux administration and shell scripting
1. Use just one command to create a directory structure where the directory sports contains a directory called footballteams which itself contains africanteam which itself contains pwdkumba.
2. Use the tree command to display your directory structure.
3. Research the following linux commands
    a) grep Grep is used for finding text patterns in a file and is the simplest  
    b) sed Sed can find and modify data
    c) awk  command is used for text processing in Linu
    
            
## CICD, Git, GitHub, GitHub Action, Infrastructure as as Code (IaC), Terraform, Packer and Ansible
1. You create a repository in GitHub called <b>myfirstrepo</b>. You then clone this repository on your local laptop. On your laptop how would you check its remote address? How would you go about changing the remote address so that it points to repository called <b>mysecondrepo</b>? ans: i will initialise this command git remote -v and do git push to know where the address is pointing to
2. You have a workflow running on GitHub Action that has the following code;
```
jobs:
  deploy_to_production:
    runs-on: ubuntu-latest
    name: deploy to production with soruce code
    steps:
      - name: Checkout GitHub Action
        uses: actions/checkout@v2

      - name: Login via Azure CLI
        uses: azure/login@v1
        with:
          creds: ${{ secrets.AZURE_CREDENTIALS }}

      - name: deploy to production step with soruce code
        uses: azure/spring-cloud-deploy@v1
        with:
          azure-subscription: ${{ env.AZURE_SUBSCRIPTION }}
          action: deploy
          service-name: <service instance name>
          app-name: <app name>
          use-staging-deployment: false
          package: ${{ env.ASC_PACKAGE_PATH }}
```
Describe what you think this code is doing.



## System Architecture and Application Design, Cloud Computing (AWS)
1. You have worked thus far with systems that you have had to download and install on your local laptop as well as systems hosted remotely on some external cloud. Describe in details the features and capabilities of all the systems (local and remote) that you have worked with thus far on this training. Draw a solution architecture diagram depicting these systems and where they fit in your solution landscape.
2. For all the systems that you have installed locally, write a manual for its installation and configuration.
3. In a general manner describe would you would interact with AWS account
4. AWS provide a public and a private area in which you could deploy your services. In which of these would you deploy the following services? 
ans: is EC2 instances 
    a) EC2 instances ans
    b) DynamoDB databases
    c) VPC network
    d) S3 buckets
    e) IAM users


## Site Reliability Engineering (SRE), Troubleshooting, Observability

1. Research on what APM (application programming monitoring)
ans: Application performance monitoring (APM) tools allow users to monitor and track the performance of particular software or web applications to identify and solve any performance issues that may arise
2. What is a system metric and why might it be useful to collect metrics?
ans: System metrics are measurement types found in the system. Each resource that can be monitored for performance, availability, reliability, and other attributes has one or more metrics about which data can be collected. Sample metrics include the amount of CPU on a node, or the amount of CPU usage on a node
3. What is an system log and why might you want to collect logs?
ans: System Log (syslog): a record of operating system events. It includes startup messages, system changes, unexpected shutdowns, errors and warnings, and other important processes. Windows, Linux, and macOS all generate syslogs.
why ans: Why is logging important? Log files (also known as machine data) are important data points for security and surveillance, providing a full history of events over time. Beyond operating systems, log files are found in applications, web browsers, hardware, and even email.


## DevOps and Agile Transformation principles and methodology

1. Communication, Collaboration and Automation and key aspects of a successful DevOps implementation. Describe why these traits are important in a DevOps transformation process.
ans: Collaboration plays a vital role in the success of a DevOps team. By fostering a culture of shared responsibility, effective communication, continuous feedback, shared goals, and knowledge sharing, teams can deliver software efficiently and improve the overall quality of their work.
2. Increased communication and collaboration in an organization is also one of the key cultural aspects of DevOps. The use of DevOps tooling and automation of the software delivery process establishes collaboration by physically bringing together the workflows and responsibilities of development and operations
2. You work for an organisation that is very keen to <b> make their work visible</b> across the organisation. What do you understand by this and how would you suggest they go about it?


## New commands logs - Enter up to ten new commands you have learnt this week

| Number      | Commands | What does it do and how might you check its effect     |
| :---        |    :----:   | :---  |
| 1  | cp -R      | to copy file |
| 2  | git status      | displays the state of the working directory and the staging area   |
| 3  | git push       | upload local repository content to a remote repository |
| 4  | git add .       | to track file   |
| 5  | control c       | to cancle  |
| 6  | chmod xx md.sh      | to give permission   |
| 7  | rw-rr--      | no permission   |
| 8  | touch       | to create file   |
| 9  | cd ../       | two step forward  |
| 10 | terraform plan       | create an execution plan   |

## Glossary of the week - Enter new technical words you have learnt this week and their meanings.

| Number   | Word | Meaning     |
| :---     | :----:   |  :---  |
| 1  | bucket      | file storage in aws cloud   |
| 2  | scripts       | collecting of command surrounded by logic   |
| 3  | awscli       | to configure source application   |
| 4  | apt       | application manager   |
| 5  | API       | central organ they gave way to the cloud   |
| 6  |container       | a place where you ran an image on platform   |
| 7  |kebernetess       | a set of computer connected together that can ran an application on aws.   |
| 8  | draw.io       | website where i can use diagram to point what i am working with and how my system interact through cicd intergration.   |
| 9  | XXXXXXXX       | YYYYYYYY   |
| 10 | XXXXXXXX       | YYYYYYYY   |

