# 
* Configuration:

Project setup
            Custom installation:
            Django:
                -> go into django dir
                -> virtualenv -p python3 vehicles_env
                -> source vehicles_env/bin/activate
                -> pip install -r requirements
                -> configure database name, user, password in vehicles/settings.py
                    DATABASES = {
                        'default': {
                            'NAME': 'your database name',
                            'USER': 'your database username',
                            'PASSWORD': 'your database password',
                        }
                    }
                # This command for initial setup only(without any migration file in repo)
                    -> python migrate.py
                #This command for existing migrations
                    -> python manage.py migrate
                -> python manage.py migrate
                -> python manage.py runserver 8000
 	   Angular6:  
                -> go into web-ui dir
                -> npm install
                -> ng serve




* Dependencies:

    Before starting setup make sure that following packages are installed in local machine
    
	    For django:				
	        -> apt-get install python-pip
	        -> apt-get install mysql-server
	        -> apt-get install mysql-client
	        -> apt-get install python3-dev
	        -> pip install virtualenv
		-> apt-get install dh-autoreconf
		-> apt-get install rabbitmq-server
		-> apt-get install svn
                -> If you got fail mysql installtion like(Command "python setup.py egg_info" failed with error code 1 in /tmp/pip-build-n3hm_k01/mysql-python/)
                     -> sudo apt-get install python-dev python3-dev
		     -> sudo apt-get install libmysqlclient-dev
              Fedora:
                  -> dnf install python-devel
                  -> dnf install python3-devel
                  -> dnf install mysql-devel
	    
	    For Angular6:
	        -> sudo apt-get install build-essential checkinstall
	        -> sudo apt-get install libssl-dev
            -> curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash
            -> curl -sL https://deb.nodesource.com/setup_10.x | sudo bash -
            -> sudo apt-get install -y nodejs
            -> sudo npm install -g @angular/cli
           
