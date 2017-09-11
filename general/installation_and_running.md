# Installation and Running

## Installation

The main server and the image analysis server can be arranged in one server or two different servers.

### The main server

1. Clone project code and install the dependencies

	    git clone git@gitlab.com:mrpike/SUCS.git
	    cd SUCS/main_server
	    chmod +x *.sh
	    ./setup.sh


2. Create a database and some tables  
(Since SUCS needs to store caches when the system runs, we need to creat a database.)
	    
	    #login to mysql
	    mysql -u[username] -p[password]
	    
	    CREATE DATABASE db_SUCS;
	    source create_database.sql
	       
	    
3. Modify SUCS/main_server/config.py according to your set.

	    #image analysis server adrress
	    __C.ADDRESSES
	    
	    #mysql username and password 
	    __C.USERNAME
	    __C.PASSWORD



### The image analysis server

1. Clone project code and install the dependencies

		#comment it when set up these two parts in one server
	    git clone git@gitlab.com:mrpike/SUCS.git    
	    
	    cd SUCS/image_analysis_server
	    chmod +x *.sh
	    ./setup.sh

2. Download directory manhole_net from [here](http://pan.baidu.com/s/1eR4wU1G) and put the whole directory into image_analysis_server.

	    #directory structure
	    SUCS
	    	|______image_analysis_server
	    					|______py-R-FCN
	    					|______images
	    					|______log
	    					|______manhole_net



## Running

### The main server

	    python main.py

### The image analysis server

	    python main.py
	    
### The webiste
1. Open web browser and input 

   address: [main_server_address]/static/login.html

2. Access with
 	
 	username: root
 	
 	password: root