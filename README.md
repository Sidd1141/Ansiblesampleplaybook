
Ansible Role: webpage


This Ansible role can be used to deploy a basic static webpage with an index.html file to a remote web server. The index.html file is assumed to be located in the files/ directory of this role.

Requirements
This role assumes that you have a remote web server that is accessible via SSH, and that you have already installed Ansible on your local machine.


Role Variables
This role has the following variables that can be customized:

Variable	Default Value	Description
localhost: 	The IP address or hostname of the web server
documentDir : 	"/var/www/sm"	- The document root directory of the web server
webPage: "index.html" - The webpage variable is the file to be hosted
packageName: "httpd"   -- The packageName variable describe the webserver on which webpage to be deployed


You can customize these variables by either creating a vars/ directory within your playbook directory, and creating a YAML file named webpage.yml, or by passing the variables in the command line when running the playbook.
