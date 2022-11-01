# DevOps-Auto-Deploy

In this project, you will prove your mastery of the following learning objectives:

- Explain the fundamentals and benefits of CI/CD to achieve, build, and deploy automation for cloud-based software products.
- Utilize Deployment Strategies to design and build CI/CD pipelines that support Continuous Delivery processes.
- Utilize a configuration management tool to accomplish deployment to cloud-based servers.
- Surface critical server errors for diagnosis using centralized structured logging.

<b>Explain the Fundamentals and Benefits of CI/CD to Achieve, Build, and Deploy Automation for Cloud-Based Software Products </b>

The deliverable should be "near-production-quality", but you should try to time-box your work to about 30 minutes. In other words, it should be good enough to submit to a manager in a real job. It should not be a messy or last-minute submission. You may use public domain or open source templates and graphics if you'd like. But please make sure the content is your own. Your presentation should be no longer than 5 slides. Your manager prefers to view presentations that are short and sweet!

Presentation should be in PDF format named "presentation.pdf" and should be included in your code repository root folder.

## directory structure relevant for the project:
``` bash
├── .circleci # You will develop the files in this directory. 
│   ├── ansible
│   └── files
├── backend  # Do not run npm commands here (on your local machine). 
│   ├── src
│   └── test
├── frontend # Do not run npm commands here (on your local machine). 
│   ├── src
│   └── types
└── util     # Files relevant for the running the app locally (Optional).
```

## Contents of the .circleci directory
1. CloudFormation templates - We have provided necessary CloudFormation templates that you can use throughout the deployment phase of your project. You can find those templates in the /.circleci/files folder. It has these files:

- cloudfront.yml - We will instruct you to use this file to manually create a stack.
- backend.yml and frontend.yml - Your CircleCI job will run these files. We will hold you along the step-by-step instructions ahead.

Note that no changes are required in three files mentioned above, except updating the EC2 key pair name and suitable AMI name in the backend.yml file later.

2. Ansible Playbooks and Roles - The /.circleci/ansible directory contains the playbook files and roles that you will develop, per instructions on the next page.

3. CircleCI config.yml file - We left a scaffolded/incomplete /.circleci/config.yml file to help you get started with CirlcCI's configuration. This file has intentionally failing/incomplete jobs. To call attention to unfinished jobs, we left some "non-zero error codes" (e.g. exit 1) for you to remove when you have finished implementing the jobs.

### Built With

- [Circle CI](www.circleci.com) - Cloud-based CI/CD service
- [CloudFormation](https://aws.amazon.com/cloudformation/) - Infrastrcuture as code
- [Ansible](https://www.ansible.com/) - Configuration management tool
- [Prometheus](https://prometheus.io/) - Monitoring tool