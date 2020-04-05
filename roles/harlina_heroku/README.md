How does this role works?
Role prepare machine to pull project from GitLab and deploy on Heroku

How?

1. Complete the variables in defaults/main.yml

app_dir: Name directory for app
repo_name: Link to repo e.g git@gitlab.com:BElluu1/BestAppEver.git
app_name: Name app on Heroku
commit_message: commited new things
ssh_key_user: SSH user which will pull project from repo
ssh_key: dest to SHH key e.g /home/belluu/.ssh/id_rsa

2. Add your credentials to Heroku in login.exp file
  You need to replace HEROKU_EMAIL and HEROKU_PASSWORD

3. Add your machine SSH key to GitLab 

4. Run your playbook like that:

ansible-playbook heroku_deploy_playbook.yml
