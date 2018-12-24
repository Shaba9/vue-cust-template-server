# Custom Vue Template (server)

## Create Custom Terminal Command

1. Create a `vue-create-cust-server.txt` file (refer above repo for content of file).
1. Allow `execute file as program` in properties.
1. Save the file wherever programs in the computer are saved (/usr/bin for Linux).

## Create Scaffolded Project
1. Create a `server` repo in GitHub.
1. Clone the repo to local.
1. `cd` into `server` repo.
1. Run the custom command in terminal:
  ```
  > vue-create-cust-server
  ```
1. Follow prompts.
1. `> code .`
1. Adjust `.env` file as desired.

## Deployment

1. Add heroku credentials locally:
    ```
    > heroku login
    ```
1. In `server`:
    1. Create heroku project `heroku create`
    1. Add postgres db
        * Dashboard
    1. Run `db` scripts against prod db
        * Additional `.env` required
    1. Add any additional env vars (`APP_SECRET`)
1. Deploy:
    1. commit!
    1. `git push heroku master`
    1. `heroku open`
    1. Profit!