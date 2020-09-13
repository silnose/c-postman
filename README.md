# Postman's course

Postman is the collaborative platform for development and testing of APIs. It builds and manages multiple APIs from you or third parties. Organize requests into collections and automate the integration of your Rest API services with your applications.

## Installing

- [x] 0- Install Postman

> sudo snap install postman

- [x] 1- Clone Repo: <https://github.com/platzi/postman-course>

- [x] 2- Install Doker

> sudo apt-get remove docker docker-engine docker-ce
> sudo apt install docker-ce
> sudo systemctl start docker
> sudo systemctl enable docker
> docker --version

Source: <https://phoenixnap.com/kb/how-to-install-docker-on-ubuntu-18-04>

- [x] 3- Install Docker Compose
  > sudo apt-get update
  > sudo apt-get upgrade
  > sudo apt install curl
  > sudo curl -L "https://github.com/docker/compose/releases/download/1.27.2/docker-compose-$(uname -s)-\$(uname -m)" -o /usr/local/bin/docker-compose
  > sudo chmod +x /usr/local/bin/docker-compose
  > docker–compose –version

Source <https://phoenixnap.com/kb/install-docker-compose-ubuntu>

- [x] 4- Run the proyect

> sudo docker-compose up -d

> sudo docker exec -it postman-course-master_web_1 bash
> cd ./project
> python manage.py migrate
> source admin_info.sh
> python manage.py loaddata courses/fixtures/initial_data.json
> exit
> sudo docker-compose stop
> sudo docker-compose up -d

- [x] 5- API URL <http://localhost:8000/api/>

- [x] 6- Admin <http://localhost:8000/admin> (CRUD)
  - superadmin
  - ThisIs@SecurePassw0rd
