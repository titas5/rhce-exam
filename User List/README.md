Create user accounts

● Download a list of users to be created from http://classroom/materials/user_list.yml
and save it to /home/student/ansible

● Using the password vault /home/student/ansible/locker.yml created elsewhere in this
exam create a playbook called /home/student/ansible/users.yml that creates user
accounts as follows:

🌕 Users which a job description of developer should be:

		■ created on managed nodes in the dev and test host group
		■ assigned the password from the pw_developer variable and should have
		password that expires after 30 days
		■ a member of supplementary group devops
🌕 Users with a job description of manager should be:

		■ created on managed nodes in the prod host group
		■ assigned the password from the pw_manager variable should have
		password that expire after 30 days
		■ a member of supplementary group manager

password should use the SHA512 hash format  
Your playbook should work using the vault password file /home/greg/ansible/secret.txt
created elsewhere in this exam
