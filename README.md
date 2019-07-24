# mirth-connect-docker

Mirth-Connect Docker Stack with 2 instances (Mirth-Connect container + Mysql container + Portainer)

## Prerequirements

- Docker
- Java

## Build Mirth-Connect docker image

  > \> docker-compose build --force-rm --no-cache --pull --parallel

## Start Mirth-Connect-Docker stack

  > \> docker-compose up -d

## Stop Mirth-Connect-Docker stack

  > \> docker-compose down

## Connect to MySQL

mirthdb1:
Use your preferred MySQL client connected to *localhost* port *3311*
(admin user: *root* / password: *password*)

mirthdb2
Use your preferred MySQL client connected to *localhost* port *3312*
(admin user: *root* / password: *password*)

### Mirth database

- database: *mirthdb*
- user: *mirth*
- password: *password*

## Connect to Mirth-Connect

Double-click on *./webstart.jnlp* to start the Mirth-Connect client
(user: *admin* / password: *admin* )

or

browse to [http://localhost:8081]() to access web client.

## Change configuration

see [./mirth-connect/README.md](./mirth-connect/README.md)

## Credits

- https://github.com/fabrom/mirth-connect-docker Fabrice Romand <fabrice.romand@gmail.com>
- [based on brandonstevens/mirth-connect docker image](https://hub.docker.com/r/brandonstevens/mirth-connect/)
