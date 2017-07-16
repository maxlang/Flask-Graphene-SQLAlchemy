# Python-Flask & Graphene-SQLAlchemy(GraphQL) Example
This is a example project for using GraphQL with Flask using Graphene-SQLAlchemy.

## Installing Requirements
Use Virtualenv and install the packages.
```
pip install -r requirements.txt
```
## Running Flask Server
Go to the root dir and run the below line in the terminal.
```
pip install -r requirements.txt
```
## Creating a new Database
Create a database(I used sqlite) with the table structure mentioned in *struct.sql* and update the database name in *database.py* file.

## Testing GraphQL
### Adding New User
```
mutation {
  createUser(name: "Rahul", email: "hello@rahulm.me", username: "rahulmfg") {
    user {
      id,
      name,
      email,
      username
    }
    ok
  }
}
```
