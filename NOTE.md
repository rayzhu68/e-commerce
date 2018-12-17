§1. setup the project
1.
sudo pip3 install Django==1.11
django-admin startproject ecommerce .
2.
/settings.py
ALLOWED_HOSTS = [os.environ.get('C9_HOSTNAME')]
3.
python3 manage.py runserver $IP:$C9_PORT
4. show favorites at the folder tree
/.bash_aliases
alias run="python3 ~/workspace/manage.py runserver $IP:$C9_PORT"
5. close and reopen terminal to refresh it to use the alias
6. hide favorites and hidden files
7. 
echo '*.sqlite3' >> .gitignore
git add --all
git commit -m "Created ecommerce project with django"

§2. Reusing An Accounts App
1. create a dir
/accounts/
2. copy all the files in Accounts-master/accounts downloaded from GitHub
3. 

§3 debug
1. in setting.py, backend:
'accounts.backends.CaseInsensitive', caused error so that it has been removed.

§4. hide secret info from github, such as env.py
echo env.py >> .gitignore