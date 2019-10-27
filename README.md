# Wordpress

Based on https://hub.docker.com/_/wordpress/



------------------------------------------------------------------------------

##Commands:

export MYSQL_DATABASE='wpdb'
export MYSQL_USER='wpuser'
export MYSQL_PASSWORD='wppass'
export WORDPRESS_DB_HOST='db'
export WORDPRESS_DB_USER=${MYSQL_USER}
export WORDPRESS_DB_PASSWORD=${MYSQL_PASSWORD}
export WORDPRESS_DB_NAME=${MYSQL_DATABASE}

docker-compose -f dc.yml up

