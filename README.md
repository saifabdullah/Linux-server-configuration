**The name of the lightsail instance created for this course is saif-aws**
**Static IP: 34.228.50.144   SSH Port : 2200    user: grader password: grader**
**Url for catalog application hosted on this server:** *catalog.saifabdullah.xyz*
**Summary List of softwares Installed:**
    - Flask
    - Python 2.7
    - Sqlalchemy
    - python pip
    - virtualenv
    - Apache 2
    - Postgresql-10
    
**Configuration changes made to run this project:**

    - Enabled catalog.conf in Apache server to run the catalog app.
    - Configured catalog.conf to serve the catalog.wsgi app.
    - Changed threads number and process number in catalog.conf.
    - Configure WSGI DaemonProcess for catalog app.
    - Configured catalog.wsgi with appropriate paths and file names.
    - Configured catalog.py and init.py to in line with catalog.wsgi
    - Configured the path  of client_secrets.json in catalog.py
    - Created a new database in the PostgreSQL named bookcatalog.
    - Configured bookcatalog' database with a new user named catalog with password 1234 
    - Give the ownership of the database to catalog user.
    - Changed book_database_setup.py, catalog.py, init.py and tonsofbook1.py with Sqlalchemy PostgreSQL wrappings.
    - Configured Amazon Lightsail Instance saif-aws with static ip 34.228.50.144
    - Configured a Web-url for the static IP namely saifabdullah.xyz
    - Configured bookcatalog app in my google developers console to serve the new adress and IP.
    - Configured client_secrets.json accordingly.
    - Changed SSH port in lightsail server to 2200.
    - Created a new user named 'grader' with password 'grader'
    - Generated a ssh-key pair for grader in my local pc and uploaded it in lightsail server
    - Created a .htacess file in webroot and edited it to deny access to the server's .git directories from the web.
    - Changed the local timezone to UTC.
    - Changed the ownership of the /var/www/catalog directory