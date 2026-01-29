FROM mysql:8.0

# Let the official entrypoint handle DB & user creation
ENV MYSQL_ROOT_PASSWORD=ExpenseApp@1
ENV MYSQL_DATABASE=transactions
ENV MYSQL_USER=expense
ENV MYSQL_PASSWORD=ExpenseApp@1

# Add SQL scripts
ADD scripts/*.sql /docker-entrypoint-initdb.d

# Do NOT switch user, use default MySQL user
# USER mysql
