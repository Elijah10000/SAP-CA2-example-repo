//The name of this branch is called 'main'

// Step 1: To create a docker network, use the following command: 'docker network create my-network'

// Step 2: To run a mysql:latest docker image with the name of db and a root password=my-secret-password, use the following command: 'docker run --name db -e MYSQL_ROOT_PASSWORD=my-secret-password -d mysql:latest'

// Step 3: To run the docker image phpmyadmin/phpmyadmin on the network previously created, mapping port 8080 to port 80 of the container, use the following command: 'docker run --name my-phpmyadmin --network my-network -e PMA_HOST=db -p 8080:80 -d phpmyadmin/phpmyadmin'

//NOTE:Replace `my-network` with the name of your network, and `my-secret-password` with a secure password of your choice. Also, you can choose any available port on your machine to map to port 80 of the container.
