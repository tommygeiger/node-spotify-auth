# Spotify web API application

Node.js and Express js web app with Spotify web API functionality. Implements Authorization Code OAuth authentication flow, referenced from [this repo](https://github.com/spotify/web-api-auth-examples).

Here are steps for running a spotify web app locally starting from this repo (requires [node.js](https://nodejs.org/en/)):

## Running Locally:
```sh
$ git clone https://github.com/tommygeiger/spotify-webapi    # or fork then clone
$ cd spotify-webapi
$ npm install
$ npm start
```
Your app should be up & running at localhost:5000.

## Setting up a Spotify Web App:

You will need to register an app and get your own credentials from the [Spotify for Developers Dashboard](https://developer.spotify.com/dashboard).

To do so, go to your Spotify for Developers Dashboard and create your application. I registered these Redirect URIs:

http://localhost:8888

http://localhost:8888/callback

Once you have created your app, replace the CLIENT_ID, CLIENT_SECRET and REDIRECT_URL in the code with the ones from your application.
