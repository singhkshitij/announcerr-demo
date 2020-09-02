# Announcerr Demo

A demo repo which sends out the changelog email to all the users with the help of [Announcer github action](https://github.com/marketplace/actions/announcerr) whenever a new app version is released !

## How it works ?
* Repo contains a [workflow file](https://github.com/singhkshitij/announcerr-demo/blob/master/.github/workflows/release.yml) that gets triggered whenever a release is made.
* This workflow files uses [Announcer github action](https://github.com/marketplace/actions/announcerr) and provides some input to the announcer such as , email username, password and list of user whom to send changelog email.
* Important step is passing the changelog file to the announcer action, which in this case is [Demo-page.html](https://github.com/singhkshitij/announcerr-demo/blob/master/demo-page.html).
* Whenever a release is made on repo , announcer gh-action gets tiggered, reads the changelog file content and sends it to all the users.

PS : To maintain privacy Gh-action is reading all the creds and emails from github secrets.
