# Rails Dev container for running Rails in VSCode

To use this example, you need to do the following:

1. Clone this repo
2. Open the repo in the VSCode's Dev Container
3. In a new Terminal
    1. run `rails new . -d postgres`
4. Add the following to the /config/databases.yml under `default: &default`
```
  host: db
  username: postgres
  password: password
  ```