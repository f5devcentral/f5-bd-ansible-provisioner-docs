Tear down lab
=============

The teardown_lab.yml playbook deletes all the sandbox instances as well as local inventory files.

To destroy all the EC2 instances after training is complete:

1. Login to the Ansible host **ansible_server_provioner**

2. Run the playbook with the same var files used to provision the infrastructure

   .. code:: 

      cd /git/workshops/provisioner
      docker run \
      -e AWS_ACCESS_KEY_ID=ABCDEFGHIJKLMNOP \
      -e AWS_SECRET_ACCESS_KEY=ABCDEFGHIJKLMNOP/ABCDEFGHIJKLMNOP \
      -v $(pwd)/../provisioner:/ansible/playbooks \
      -v /git:/ansible/vars \
      ansible_workshop:dockerfile teardown_lab.yml -e @/ansible/vars/f5_vars.yml

   Alternatively, if using an `AWS CLI credential file <https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html>`_ a mapped volume could be used. For example:

   .. code::
      
      cd /git/workshops/provisioner
      docker run \
      -v ~/.aws/credentials:/root/.aws/credentials \
      -v $(pwd)/../provisioner:/ansible/playbooks \
      -v /git:/ansible/vars \
      ansible_workshop:dockerfile teardown_lab.yml -e @/ansible/vars/f5_vars.yml
