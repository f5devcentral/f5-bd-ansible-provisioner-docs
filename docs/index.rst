F5 Automation Sandbox
======================

Introduction:
----------------------
The F5 Solution Sandbox provides a demo environment to get familiar with the solutions that F5 provides in security, performance, and visibility. Users can use this environment to try automation solutions, build demos and proof of concepts. Using the scenarios provided, users will be able to experience how F5 adds value and integrates into your build environment seamlessly.

The F5 Solution Sandbox delivers a few common scenarios to help you learn more:

* Virtaul server deployment with redirection of HTTP to HTTPS traffic to enforce secured connections
* An automated SSL certificate update scenario to manage key updates
* Web server pool membership management as a server maintenance scenario
* A Web Application Firewall policy management with URL and IP adress blocking scenario

Best of all, these scenarios are all powered with simple Ansible scripts that require zero knowledge of F5 configuration. 

Solution Architecture:
-------------------------
The solution environment has two main components:
1.	The F5 Sandbox Provisioner – powered by Ansible and delivered via Docker containers, this sets up the architecture and environment. The architecture is fairly simple with some key components such as a F5 BIG IP Virtual Edition instance, an Ansible node, and a pair of web servers. You can learn more about the provisioned components in the next page.

2.	Solution use cases – overlaid onto the environment are the specific solution demos referenced above. Over time, we’ll add more solution demos to the architecture. More documentation for each use case is available 'here <https://clouddocs.f5.com/training/fas-ansible-use-cases/'.

Requirements
-------------
Before you get started, here are some minimum requirements to start using this project: 

* Knowledge on using Linux environments 
* Knowledge on how to run docker containers    
* It’s helpful if you have some knowledge or familiarity with how F5 protects and manages the security and performance of applications (though no configuration knowledge is required). 
* An AWS account and the knowledge to operate it  
* Ability to spin up resources in AWS (w.r.t. cost, access etc.).  

Filing Issues and Getting Help
------------------------------
If you come across a bug or other issue when using this project use `GitHub Issues <https://github.com/f5devcentral/FAS-provisioner/issues>`_ to submit an issue for our team. You can also see the current known issues on that page, which are tagged with a purple Known Issue label.

License and Warranty
---------------------
This software is supplied under the MIT license, strictly for testing purposes, and with absolutely no warranty whatsoever.
Please see the LICESNSE.txt file for details.

F5 Networks Contributor License Agreement
-----------------------------------------
Before you start contributing to any project sponsored by F5 Networks, Inc. (F5) on GitHub, you will need to sign a Contributor License Agreement (CLA).

If you are signing as an individual, we recommend that you talk to your employer (if applicable) before signing the CLA since some employment agreements may have restrictions on your contributions to other projects. Otherwise by submitting a CLA you represent that you are legally entitled to grant the licenses recited therein.

If your employer has rights to intellectual property that you create, such as your contributions, you represent that you have received permission to make contributions on behalf of that employer, that your employer has waived such rights for your contributions, or that your employer has executed a separate CLA with F5.

If you are signing on behalf of a company, you represent that you are legally entitled to grant the license recited therein. You represent further that each employee of the entity that submits contributions is authorized to submit such contributions on behalf of the entity pursuant to the CLA.

Now that you are familiar with the prerequisites of the project, click *Next* to get started with the Provisioner.

.. toctree::
   :glob:
   :maxdepth: 2
   :hidden:

   build_environment.rst
   ansible_use_cases_and_labs.rst
   teardown.rst
   faq.rst
