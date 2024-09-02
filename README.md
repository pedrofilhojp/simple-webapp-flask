# Simple Web Application
Esta é uma aplicação simples usnado o [Python Flask] (http://flask.pocoo.org/) e [Mysql] (https://www.mysql.com/)
Utilizamos esta aplicação para demonstrar seu uso em construção de containeres Docker e Ansible Playbook

Os seguintes passos são requeridos
  - **Instale todas as dependências requeridas**
  - **Instale e configure o webserver**
  - **Inicie o webserver**
   
## 1. Instalando todas as dependencias requeridas
  
  Python and its dependencies
  ```bash
  apt-get install -y python3 python3-setuptools python3-dev build-essential python3-pip default-libmysqlclient-dev
  ```
   
## 2. Instale e configure o webserver

Install Python Flask dependency
```bash
pip3 install flask
pip3 install flask-mysql
```

- Copy `app.py` or download it from a source repository
- Configure database credentials and parameters 

## 3. Inicie o webserver

Start web server
```bash
FLASK_APP=app.py flask run --host=0.0.0.0
```

## 4. Teste

Open a browser and go to URL
```
http://<IP>:5000                            => Welcome
http://<IP>:5000/how%20are%20you            => I am good, how about you?
```
