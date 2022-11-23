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

Click on ‘Add variable’ and input the variable name as API_KEY and the value as the bot’s API token and save your settings.

# 2. Setting webhooks for our bot

Now, with our endpoint ready, all that is left to do is to set the webhook of our bot to our custom endpoint.

With our bot API token, and the URL of our new worker (which should be ending with workers.dev), substitute the values into this URL and simply copy and paste it into your browser and enter

https://api.telegram.org/bot<replace with bot api token>/setWebhook?url=<replace with our worker url>


If you see this as a response, you’re all set!

{"ok":true,"result":true,"description":"Webhook was set"}
