
# Login Credentials
- **Role: User**
  - Username: jonas
  - Password: 1234
- **Role: Agent**
  - Username: samu2k
  - Password: 1234
- **Role: Admin**
  - Username: pessoa
  - Password: 1234

# Project Execution Commands
To run the project, follow these commands:

```shell
git clone https://github.com/FEUP-LTW-2023/project-ltw04g03.git
cd project-ltw04g03
git checkout final-delivery-v1
sqlite3 tickets.db < tickets.sql
sqlite3 tickets.db < populate.sql
php -S localhost:9000
