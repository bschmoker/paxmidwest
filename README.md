Manage your local gaming conference in a flyover state

## Requirements
- [Sign up for Dev account on App Engine][1]

- [Install App Engine Python SDK](https://cloud.google.com/appengine/downloads?hl=en_US#Google_App_Engine_SDK_for_Python)

## APIs
- [Google Cloud Endpoints][3]

## Setup Instructions
1. Update the value of `application` in `app.yaml` to the app ID you
   have registered in the App Engine admin console and would like to use to host
   your instance of this sample.
1. Update the values at the top of `settings.py` to
   reflect the respective client IDs you have registered in the
   [Developer Console][4].
1. Update the value of CLIENT_ID in `static/js/app.js` to the Web client ID
1. (Optional) Mark the configuration files as unchanged as follows:
   `$ git update-index --assume-unchanged app.yaml settings.py static/js/app.js`
1. Run the app with the devserver using `dev_appserver.py DIR`, and ensure it's running by visiting your local server's address (by default [localhost:8080][5].)
1. (Optional) Generate your client library(ies) with [the endpoints tool][6].
1. Deploy your application with `appcfg.py -A paxmidwest update app.yaml --noauth_local_webserver`


[1]: https://developers.google.com/appengine
[3]: https://developers.google.com/appengine/docs/python/endpoints/
[4]: https://console.developers.google.com/apis/credentials
[5]: https://localhost:8080/
[6]: https://developers.google.com/appengine/docs/python/endpoints/endpoints_tool
