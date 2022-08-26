# umami on Render

This repository allows you to deploy the latest umami software (v1.37.0) on Render.

Follow these steps:



1. Login onto your Render [Dashboard](https://dashboard.render.com/)

2. Click on +New/Web Service

3. Connect to the Public Repository: [thomascenni/umami](https://github.com/thomascenni/umami)

4. Click on Continue, select a name for your web service, for example "umami"

5. Before creating the service, click on "Advanced" and setup the two environment variables:
   
   1. DATABASE_URL, with the connection string coming from your PostgreSQL Render service
   
   2. HASH_SALT, with a random generated string



Once the web service is deployed, you'll be redirected to the admin page, login with user "admin" and password "umami".

Alternatively:

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/thomascenni/umami)
