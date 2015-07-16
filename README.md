# awsCurse
Curso AWS


/var/apps/talentum-2015

user: ubuntu


sudo nodejs app.js


________________
cmd

aws --version
aws .configure


eu-west-2
json

C:\Users\Migue>aws ec2 run-instances --image-id ami-5189a661 --count 1 --instanc
e-type t2.micro --key-name TalentumRocks --security-group-ids sg-8e9a59ea --subn
et-id subnet-0cd37855




EC2 
______________________________

sudo apt-get update
sudo apt-get install nodejs git npm -y
sudo npm install connect serve-static
sudo git clone https://github.com/denisroldan/talentum-2015-examples

root@ip-10-0-0-213:/home/ubuntu# apt-get update && apt-get upgrade && apt-get dist-upgrade apt-get update && apt-get upgrade && apt-get dist-upgrade



DB
______________
cerrar puerto 22 a todas las ips  o instalar firewall
apt-get install ufw
ufw allow 22
ufw allow 80
ufw limit 22 //limita las conexiones a u puerto a 6, si el servidor fallas 6 veces te baena
ufw enable
ufw status

apt-get install mysql-sever libmysqlclient-dev
pass:admin
 
apt-get install python3 python-virtualenv
apt-get install python3-dev build-essential
apt-get install nginx
apt-get install uwsgi uwsgi-plugin-python

mkdir /var/apps/quiz
cd /var/apps/quiz
git clone https://github.com/denisroldan/talentum-2015-examples repo
mkdir logs
mkdir static


virtualenv env -p python3
 source env/bin/activate

cat /etc/hosts
cat /etc/hostname
si quieres añadir 127.0.0.1 ip-10-0-0-142 en /etc/hosts

cd repo 
git checkout no-rel


cd ..
ls -la

en el dirctoriocode python manage.py collectstatic

 nano gamequiz/settings.py

mysql -u root -p
:admin
			create database quiz;
			exit
contrasela en setting.py de la basede datos
 pip install -r requirements.txt (en code)
 python manage.py collectstatic
python manage.py migrate

 python manage.py loaddata data.json
cp quiz.ini /etc/uwsgi/apps-enabled/

 cp /var/apps/quiz/repo/python/demo-django/server/nginx.conf  /etc/nginx/sites-enabled/default
 service nginx restart
service uwsgi restart

apt-get purge uwsgi-plugin-python
apt-get install uwsgi-plugin-python3
apt-get install python-dev
 git checkout no-rel
git pull
service uwsgi restart
service nginx restart





