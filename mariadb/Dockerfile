FROM mariadb:latest

# Set environment variables
ENV MYSQL_ROOT_PASSWORD=db_root_password
ENV MYSQL_DATABASE=mydatabase
ENV MYSQL_USER=db_user
ENV MYSQL_PASSWORD=db_password

# Copy the SQL script to initialize the database
COPY init.sql /docker-entrypoint-initdb.d/

# Expose the default MySQL port
EXPOSE 3306
