# GeoSlack
Slack integration that lets your Slack team plot and share their locations on a map
![GeoSlack](https://dl.dropboxusercontent.com/s/kellfmkvwinxm11/01GeoSlack.png?dl=0)

## Configuration and Installation

1. Generate a Slack Incoming Webhook
   - Login to Slack
   - Go to this [link](https://api.slack.com/incoming-webhooks#share_your_incoming_webhook_as_a_slack_app)
   - Click on "..__incoming webhook integration__" near the top paragraph of the page.  Then you'll see this page..

   ![IncomingWebhook01](https://dl.dropboxusercontent.com/s/3jjkxvwoniuwglj/webhooks01.PNG?dl=0)

    - Click the green button (see above), then you'll see this page (below).  You'll have to scroll down to the __Integration Settings__ to see it:

   ![IncomingWebHook02](https://dl.dropboxusercontent.com/s/6r4hy2n1g3x69s5/SlackWebhookIncoming.PNG?dl=0)

2. Click the button below to deploy the app to your Heroku account.

   [![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

   Name your app. After it has been deployed, scroll near the top and find the app's  __Settings__. Add Heroku config variables for:
   - __`APP_URL`__- Format of URL is `http://<your_heroku_app_url>/geoloc.htm`
   - __`SLACK_INCOMING_WEBHOOK_URL`__ - From Step 1 above, but __SHOULD NOT__ include the http://hooks.slack.com hostname.  See example below

    ![HerokuConfigVars](https://dl.dropboxusercontent.com/s/b42hgobyj3dq1lh/03GeoSlack.PNG?dl=0)

3. Set up a Slack Outgoing Webhook.  
   - Go to this [link](https://api.slack.com/outgoing-webhooks)
   - Click on "..__outgoing webhook integration__" near the top paragraph of the page.  It will take you to a page with a big green button that says __Add Outgoing Webhook Integration__.  Click that.  You will be then taken to this page..
    ![OutgoingWebhook](https://dl.dropboxusercontent.com/s/c8cg62s0f0f0q7p/SlackWebhookOutgoing.PNG?dl=0)

    - URL(s) - Format of URL is `http://<your_heroku_app_url>/slack`

## Questions, Comments, Suggestions
Email me at chris.ismael@gmail.com

## License
The MIT License (MIT)
Copyright (c) 2015 Chris Ismael

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
