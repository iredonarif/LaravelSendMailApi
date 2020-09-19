## About the App (send-mail-api)

This is a laravel project for sending mails.
The app is developped like a webservice and will be used by another apps.

All the logic for sending mails are implemented in this webserivice. So if an app needs to send emails; it will only called the endpoint provided by this webservice for sending mails.

Any application must be registered in the webservice database before being able to call the webservice.
An app will be registred with these informations: name, email.

After registration, a token will be generated and will be send to the app (by using the specified email address).

This token will be used as access_token in the request header when calling send-mail-api.

## Note
I used mailgun as mail driver. I haven't provided my mailgun account's credentials in this repo. So if you want to clone and test will have to set your mailgun credentials.
Thanks 😺!

