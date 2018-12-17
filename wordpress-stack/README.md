# Wordpress stack with phpmyadmin

Files used: [
"docker-compose.yml",
".dockerignore"
]

Run the next commands in the same folder as the YML file

To start the server service execute:

`docker-compose up -d`

**Note 1:** On the first run the containers take some time to start!

To stop the service execute:

`docker-compose down`

This `docker-compose.yml` will create two (2) new folders:

- A `/wp` folder that maps the `/var/www/html` inside the WordPress container
- A `/db` folder that maps the `/var/lib/mysql` inside the MySQL container

**Note 2:** I added a `.dockerignore` file if you decide to not save the containers files, instead you may decide to user and import/export WordPress plugin to save all your configs, or you may decide to save only the `wp/wp-content` if you are developing a theme or a plugin!
