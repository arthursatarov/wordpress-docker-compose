# wordpress-docker-compose

## Installation
1. Clone this repository to your local machine
2. Use the ```cp .env.example .env``` command to copy the environment variables file and edit it.
3. Start the container with the command ```docker-compose up -d```
4. Change permissions to the folder ```sudo chmod 777 -R web mysql```

To have Git ignore ```chmod``` changes, update local git config with the command ```git config --local core.fileMode false```
