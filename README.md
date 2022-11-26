Prerequisites

  Key pair - An AWS EC2 key pair "udacity.pem" already created in AWS Console and downloaded to local machine
  A public Github repository set up in the CircleCI.
  AWS Access keys saved in the CircleCI project settings.
  Finished the previous Exercise: Infrastructure Creation and Exercise: Remote Control Using Ansible, and have the following files in the repo and local:

  └── template.yml           # Change the KeyName and ImageID property value
  ├── ansible.cfg            # Disables host_key_checking 
  ├── inventory              # Or it could be inventory.txt
  ├── main.yml               # Playbook file from the Exercise: Remote Control Using Ansible
  └── roles
  │   └── setup
  │       ├── files
  │       │   └── index.js
  │       └── tasks
  │           └── main.yml
  └── .circleci
      └─── config.yml        # Should have the create_infrastructure Job


  The Ansible Playbook above is responsible for configuring the EC2 instance and copy over the files/index.js file.

  EC2 Ubuntu instance - An Ubuntu EC2 instance running in the AWS account and use "udacity" key pair.