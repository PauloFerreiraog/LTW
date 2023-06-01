
## Login Credentials
- **Role: User**
  - Username: jonas
  - Password: 1234
- **Role: Agent**
  - Username: samu2k
  - Password: 1234
- **Role: Admin**
  - Username: pessoa
  - Password: 1234

##Project Featurers

### General Features

- All users can (users can simultaneously be clients and agents):
  - Register a new account.
  - Login and Logout.
  - Edit their profile (at least name, username, password, and e-mail).

### Client Features

- Clients are be able to:
  - Submit a new ticket optionally choosing a department (e.g., "Accounting").
  - List and track tickets they have submitted.
  - Reply to inquiries (e.g., the agent asks for more details) about their tickets and add more information to already submitted tickets.

### Agent Features

- Agents are be able to (they are also clients):
  - List tickets from their departments (e.g., "Accounting"), and filter them in different ways (e.g., by date, by assigned agent, by status, by priority, by hashtag).
  - Change the department of a ticket (e.g., the client chose the wrong department).
  - Assign a ticket to themselves or someone else.
  - Change the status of a ticket. Tickets can have many statuses (e.g., open, assigned, closed); some may change automatically (e.g., ticket changes to "assigned" after being assigned to an agent).
  - Edit ticket hashtags easily (just type hashtag to add (with autocomplete), and click to remove).
  - List all changes done to a ticket (e.g., status changes, assignments, edits).
  - Manage the FAQ and use an answer from the FAQ to answer a ticket.

### Admin Features

- Admins are be able to (they are also agents):
  - Upgrade a client to an agent or an admin.
  - Add new departments, statuses, and other relevant entities.
  - Assign agents to departments.
  - Control the whole system.



## Project Execution Commands
To run the project, follow these commands:

```shell
git clone https://github.com/PauloFerreiraog/LTW.git
cd LTW
git checkout final-delivery-v1
sqlite3 tickets.db < tickets.sql
sqlite3 tickets.db < populate.sql
php -S localhost:9000


