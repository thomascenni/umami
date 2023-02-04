# Umami on Render

This repository allows you to deploy the latest <a href="https://umami.is/" target="_blank">Umami software</a> (v1.40.0) on Render.

## Automatic Deploy
[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/thomascenni/umami)


## Manual Deploy

1. Login onto your Render [Dashboard](https://dashboard.render.com/)

2. If you don't have a PostgreSQL database running, deploy a new one with the button "+New/PostgreSQL" 

3. Click on "+New/Web Service" to host Umami application

4. Connect to this public repository: [https://github.com/thomascenni/umami](https://github.com/thomascenni/umami)

5. Click on Continue, select a name for your web service, for example "umami"

6. Before creating the service, click on "Advanced" and setup the two environment variables:
   
   1. DATABASE_URL, with the connection string coming from your PostgreSQL service (point 2)
   2. HASH_SALT, with a random generated string


Once the web service is deployed, you'll be redirected to the admin page, login with user "admin" and password "umami".
