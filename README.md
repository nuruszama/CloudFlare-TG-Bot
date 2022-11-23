# CloudFlare-TG-Bot
Table of Contents:

Creating a new Cloudflare Worker

Setting webhooks for our Telegram bot

# 1. Creating a new Cloudflare Worker

Navigate to dash.cloudflare.com and login (or sign up)

On the sidebar, click on ‘Workers’

Click on ‘Create a service’ to create your new worker

Enter a name for your new worker and select the ‘HTTP handler’ as the starter, and click on ‘Create service’

Once your service has been created, click on ‘Quick Edit’ to edit your worker directly in the browser

Now, in your editor, you should be seeing the default code for a new Cloudflare worker.

Change  the codes as in echo

Go back to the your worker’s dashboard by clicking on ‘Save & Deploy’ and then exiting out of the editor.

Under the settings panel, click on variables. Here you can set the environment variable for the worker.
