Ansible Automation Workshops
============================

Introduction:
----------------------
The Ansible Automation Workshops provides a demo (Sandbox) environment to get familiar with various solutions.  This includes F5 products in security, performance, and visibility. Users can use this environment to try F5 automation solutions, build demos and proof of concepts. Using the scenarios provided, users will be able to experience how F5 adds value and integrates into your build environment seamlessly.

The Ansible Automation Sandbox delivers a few common scenarios to help you learn more:

* Virtual server deployment with redirection of HTTP to HTTPS traffic to enforce secured connections
* An automated SSL certificate update scenario to manage key updates
* Web server pool membership management as a server maintenance scenario
* A Web Application Firewall policy management with URL and IP adress blocking scenario

Best of all, these scenarios are powered with simple Ansible scripts that require zero knowledge of F5 configuration. 

Solution Architecture:
-------------------------
The solution environment has two main components:

1.	The Ansible Workshop Provisioner – powered by Ansible and delivered via Docker containers, this sets up the architecture and environment. The architecture is fairly simple which includes some key components such as a F5 BIG IP Virtual Edition instance, an Ansible node, and a pair of web servers. You can learn more about the provisioned components in the next page.

2.	Solution use cases – overlaid onto the environment are the specific solution demos referenced above. Over time, we’ll add more solution demos to the architecture. More documentation for each use case is available `here <https://clouddocs.f5.com/training/fas-ansible-use-cases/>`_.

Requirements
-------------
Here are some minimum requirements to start using this project: 

* Knowledge on using Linux environments 
* Knowledge on how to run docker containers    
* It’s helpful if you have some knowledge or familiarity with how F5 protects and manages the security and performance of applications (though no configuration knowledge is required). 
* An AWS account and the knowledge to operate it  
* Ability to spin up resources in AWS (w.r.t. cost, access etc.).  

Filing Issues and Getting Help
------------------------------
If you come across a bug or other issue when using this project use `GitHub Issues <https://github.com/ansible/workshops/issues/>`_ to submit an issue. You can also see the current known issues on that page, which are tagged with a orange "f5-workshop" label.

License and Warranty
---------------------
This software is supplied under the MIT license, strictly for testing purposes, and with absolutely no warranty whatsoever.
Please see the LICESNSE.txt file for details.


Now that you are familiar with the prerequisites of the project, click *Next* to get started with the Provisioner.

.. toctree::
   :glob:
   :maxdepth: 2
   :hidden:

   build_environment.rst
   ansible_use_cases_and_labs.rst
   teardown.rst
   faq.rst
