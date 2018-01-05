------------prerequisite---------------


--Install ansible and pip RPM
# yum install ansible python-pip

--Install awscli and boto moudule using pip
# pip install boto3 awslci boto

--Congiure AWS CLI with your credentials
# aws configure
provide access, secret key and region as us-west-2

--Create a new Key Pair in AWS console and download in to your local machine

--Replace key_name in aws_instances_creation.yml 
===
key_name: PRAKASH
to 
key_name: your_key_pair_name
====


--Update anisble.cfg file which is cloned from the gitub
===
roles_path    = /root/devops/roles/ 
to
roles_path    = current_path_where_git_is_cloned

private_key_file = PRAKASH.pem
to
private_key_file = current_path_where_your_pem_key_is_placed
=====

