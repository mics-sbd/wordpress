# Wordpress

Based on [Docker image for Wordpress 1.x](https://hub.docker.com/_/wordpress) and Alpine.



------------------------------------------------------------------------------

## Commands:

Environment variables are needed to initialize wordpress and point it to a database.

See the [Docker image for Wordpress 1.x](https://hub.docker.com/_/wordpress) for additional information about supplying a file with environment variables for the `docker-entrypoint.sh`.

~~~
export MYSQL_DATABASE='wpdb'
export MYSQL_USER='wpuser'
export MYSQL_PASSWORD='wppass'
export WORDPRESS_DB_HOST='db'
export WORDPRESS_DB_USER=${MYSQL_USER}
export WORDPRESS_DB_PASSWORD=${MYSQL_PASSWORD}
export WORDPRESS_DB_NAME=${MYSQL_DATABASE}

docker-compose -f dc.yml up

~~~
