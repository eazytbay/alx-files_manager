

**0x04. Files Manager**

This is a straightforward file management API developed using Express, MongoDB, Redis, Bull, and Node.js.

**Requirements**

- **Applications**
  - **Node.js**
  - **Yarn** (the package manager/resource negotiator)

- **APIs**
  - A Google API needs to be configured with at least an email sending scope and a valid URL, such as `http://localhost:5000/`, set as one of the redirect URIs. Ensure that the `credentials.json` file is placed in the root directory of this project.

- **Environment Variables**
  - Required environment variables should be defined in a `.env` file with each entry following the format `Name=Value`. Below are the environment variables that this server will use:

| Name                | Required | Description                                                                         |
|---------------------|----------|-------------------------------------------------------------------------------------|
| `GOOGLE_MAIL_SENDER`| Yes      | The email address responsible for sending emails to users.                          |
| `PORT`              | No       | (Default: 5000) The port on which the server will listen.                            |
| `DB_HOST`           | No       | (Default: localhost) The database host.                                             |
| `DB_PORT`           | No       | (Default: 27017) The database port.                                                 |
| `DB_DATABASE`       | No       | (Default: files_manager) The database name.                                         |
| `FOLDER_PATH`       | No       | (Default: `/tmp/files_manager` for Linux/Mac OS X and `%TEMP%/files_manager` for Windows) The directory where files are stored locally. |

**Installation**

1. Clone this repository and navigate to the cloned directory.
2. Install the required packages using `yarn install` or `npm install`.

**Usage**

- Start the Redis and MongoDB services on your system, then run `yarn start-server` or `npm run start-server`.

**Testing**

- Create a separate `.env` file for testing, name it `.env.test`, and store the appropriate environment variable values for testing.
- Run `yarn test` or `npm run test` to perform end-to-end (E2E) tests.

**Authors**
EZEKIEL OLUWATOBI FOLARIN
