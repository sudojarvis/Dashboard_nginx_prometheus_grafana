# Description: This is a simple dashboard for nginx with prometheus and grafana

To run this project you need to have docker and docker-compose installed on your machine.

Before running the project you need to to install docker and docker-compose.

# How to run

1. Clone this repository
2. Run `docker-compose up -d`
3. To open grafana dashboard your browser and go to `http://localhost:3000` and login with `admin` and `admin` as username and password respectively.
4. To open prometheus dashboard your browser and go to `http://localhost:9090`
5. To check nginx status go to `http://localhost:8080`.
6. To check the status of telegraf go to `http://localhost:9125`
7. T0 get ip_adress of telegraf from docker run `docker inspect -f telegraf`. And replace the ip_address in `prometheus.yml` file.

# How to stop

1. Run `docker-compose down`

# How to remove

1. Run `docker-compose down -v`

# How to restart

1. Run `docker-compose restart`

# How to check logs

1. Run `docker-compose logs -f`
