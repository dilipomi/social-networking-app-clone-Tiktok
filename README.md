

![image](https://raw.githubusercontent.com/DataStax-Examples/astra-tik-tok/master/screenshot.jpg)


## Objectives
* Work through a video tutorial to build a simple Tik-Tok clone
* Leverage Netlify and DataStax Astra DB
  
## Prerequisites
Let's do some initial setup by creating a serverless(!) database.

### DataStax Astra
1. Create a [DataStax Astra account](https://dtsx.io/2WMxoBQ) if you don't already have one:
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-register-basic-auth.png)

2. On the home page. Locate the button **`Create Database`**
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-dashboard.png)

3. Locate the **`Get Started`** button to continue
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-select-plan.png)

4. Define a **database name**, **keyspace name** and select a database **region**, then click **create database**.
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-create-db.png)

5. Your Astra DB will be ready when the status will change from *`Pending`* to **`Active`** 💥💥💥 
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-db-active.png)

6. After your database is provisioned, we need to generate an Application Token for our App. Go to the `Settings` tab in the database home screen.
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-db-settings.png)

1. Select `Admin User` for the role for this Sample App and then generate the token. Download the CSV so that we can use the credentials we need later.
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-db-settings-token.png)

1. After you have your Application Token, head to the database connect screen and copy the connection information that we'll need later. We'll replace `ASTRA_DB_APPLICATION_TOKEN` with the `Token` value that is part of your Application Token.
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-db-connect.png)



## 🚀 Getting Started Paths:
*Make sure you've completed the [prerequisites](#prerequisites) before starting this step*
  - [Running on your local machine](#running-on-your-local-machine)

### Running on your local machine
1. Create a `.env` file and fill it with values from the `.env.sample` file.

2. Make sure the package dependencies are installed
```sh
# install dependencies
npm install
```

3. Then, start the app in dev mode. Changes in the `src` or `functions` directories will trigger reloads.
```sh
# start in dev mode
npm run dev
```
<!--- ENDEXCLUDE --->
