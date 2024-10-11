# User Authentication System

## Overview
The **User Authentication System** is a Java-based application designed to manage user registration and login functionalities using an SQL database. It provides a user-friendly interface through Java AWT and Swing, allowing users to securely access their account information.

## Features
- **User Registration**: Users can create new accounts with a username, email, and password.
- **User Login**: Registered users can log into their accounts using their credentials.
- **Data Persistence**: User information is securely stored in an SQL database.
- **GUI Interface**: Built with Java AWT and Swing for an intuitive user experience.
- **Password Protection**: Passwords are securely managed within the application.

## Technology Stack
- **Programming Language**: Java
- **GUI**: Java AWT, Java Swing
- **Database**: MariaDB (or compatible SQL database accessed via JDBC)
- **Java Collections**: For managing in-memory data

## Database Details

### Database Name
- `sqlDB`

### Tables
Table present in the `sqlDB` database:

1. **userData** (utilized for user authentication)

### `userData` Table Schema
The `userData` table is crucial for managing user authentication, and it has the following schema:

| Field            | Type          | Null | Key | Default | Extra          |
|------------------|---------------|------|-----|---------|----------------|
| `user_id`        | int(11)      | NO   | PRI | NULL    | auto_increment |
| `user_gmail`     | varchar(50)  | NO   |     | NULL    |                |
| `user_name`      | varchar(20)  | NO   | UNI | NULL    |                |
| `user_password`  | varchar(20)  | NO   |     | NULL    |                |

### SQL Query for Schema
You can create the `userData` table using the following SQL query:

```sql
CREATE TABLE userData (
    user_id INT(11) NOT NULL AUTO_INCREMENT,
    user_gmail VARCHAR(50) NOT NULL,
    user_name VARCHAR(20) NOT NULL UNIQUE,
    user_password VARCHAR(20) NOT NULL,
    PRIMARY KEY (user_id)
);
```
### Screenshots
- SignIn

![sin](https://github.com/user-attachments/assets/5e1d9bf5-3ccc-47ac-aee8-7aada2116328)

- SignUp

![sup](https://github.com/user-attachments/assets/fb957c35-f843-49e0-a749-3c5a9845c1d4)

- Other

![inv](https://github.com/user-attachments/assets/55f9bedb-d6bb-487c-a16b-52939b328ce8)
![req](https://github.com/user-attachments/assets/39ef8441-1a11-42f0-ac60-674f135940fa)


### Cloning the Repository

Clone the repository to your local machine using the following command:

```bash
git clone https://github.com/voidAasif/userAuth.git
