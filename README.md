# DevOps-Auto-Deploy

In this project, you will prove your mastery of the following learning objectives:
- Utilize Deployment Strategies to design and build CI/CD pipelines that support Continuous Delivery processes.
- Utilize a configuration management tool to accomplish deployment to cloud-based servers.
- Surface critical server errors for diagnosis using centralized structured logging.

## Directory structure relevant for the project:
``` bash
├── .circleci
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
1. CloudFormation templates - use throughout the deployment phase of this project: <b>cloudfront.yml</b> - use this file to manually create a stack.<b>backend.yml and frontend.yml</b> - CircleCI job will run these files.

2. Ansible Playbooks and Roles - The /.circleci/ansible directory contains the playbook files and roles that you will develop, per instructions on the next page.

3. CircleCI config.yml file

### Built With

- [Circle CI](www.circleci.com) - Cloud-based CI/CD service
- [CloudFormation](https://aws.amazon.com/cloudformation/) - Infrastrcuture as code
- [Ansible](https://www.ansible.com/) - Configuration management tool
- [Prometheus](https://prometheus.io/) - Monitoring tool