§1. setup the project
1.
sudo pip3 install Django==1.11
django-admin startproject ecommerce .
2.
/settings.py
ALLOWED_HOSTS = [os.environ.get('C9_HOSTNAME')]
3.
python3 manage.py runserver $IP:$C9_PORT
4. 
/.bash_aliases
alias run="python3 ~/workspace/manage.py runserver $IP:$C9_PORT"
