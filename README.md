How does this role works?
Role prepare machine to pull project from GitLab and deploy on Heroku

How?

1. Complete the variables in defaults/main.yml

<b>app_dir:</b> Name directory for app  
<b>repo_name:</b> Link to repo e.g git@gitlab.com:BElluu1/BestAppEver.git  
<b>app_name:</b> Name app on Heroku  
<b>commit_message:</b> commited new things  
<b>ssh_key_user:</b> SSH user which will pull project from repo  
  <b>ssh_key:</b> dest to SHH key e.g /home/belluu/.ssh/id_rsa  

2. Add your credentials to Heroku in login.exp file  
  You need to replace <b>HEROKU_EMAIL</b> and <b>HEROKU_PASSWORD</b>  

3. Add your machine SSH key to GitLab   

4. Run your playbook like that:  

<b>ansible-playbook heroku_deploy_playbook.yml</b>  
