# FILES MANAGER

Joint project between Wycliffe Ochieng and Joash Mobinda

A simple file management API built with Express, MongoDB, Redis, Bull, and Node.js.

## REQUIREMENTS

### Applications

+ Node.js
+ Yarn (the package manager/resource negotiator)

### APIs

+ A Google API should be created with at least an email sending scope and a valid URL (e.g.; `http://localhost:5000/`) should be one of the redirect URIs. The `credentials.json` file should be stored in the root directory of this project.

### ENVIRONMENT VARIABLES

The required environment variables should be stored in a file named `.env` and each line should have the format `Name=Value`. The table below lists the environment variables that will be used by this server:

| Name | Required | Description |
|:-|:-|:-|
| GOOGLE_MAIL_SENDER | Yes | The email address of the account responsible for sending emails to users. |
| PORT | No (Default: `5000`)| The port the server should listen at. |
| DB_HOST | No (Default: `localhost`)| The database host. |
| DB_PORT | No (Default: `27017`)| The database port. |
| DB_DATABASE | No (Default: `files_manager`)| The database name. |
| FOLDER_PATH | No (Default: `/tmp/files_manager` (Linux, Mac OS X) & `%TEMP%/files_manager` (Windows)) | The local folder where files are saved. |

## INSTALLATION

Clone this repository and switch to the cloned repository's dire    ctory.
Install the packages using `yarn install` or `npm install`.

## USAGE

Start the Redis and MongoDB services on your system and run `yarn     start-server` or `npm run start-server`.

## TESTS

Create a separate `.env` file for the tests named `.env.test` an    d store the value of the environment variables for the testing eve    nt in it.
+ Run `yarn test` or `npm run test` to execute the E2E tests.

## DOCUMENTATION

+ Generate OpenAPI documentation with [**apidoc**](https://www.npmjs.com/package/apidoc).          
