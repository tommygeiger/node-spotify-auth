# Spotify API web application

Node.js and Express js web app with Spotify API functionality. Implements "authorization code" OAuth authentication flow, borrowed from [this repo](https://github.com/spotify/web-api-auth-examples).

Here are steps for running a Spotify web app locally starting from this repo (requires [Node.js](https://nodejs.org/en/)):

## Setting up local Node.js environment:
```
$ git clone https://github.com/tommygeiger/spotify-webapi    # or fork then clone
$ cd spotify-webapi
$ npm install
$ npm start
```
Your app should be up and running at localhost:5000 (but it's not going to work yet)

## Setting up a Spotify web app:

You'll need to register a Spotify app and add your own credentials to the code. First go to the [Spotify for Developers Dashboard](https://developer.spotify.com/dashboard) and create an application. Then add these two redirect URIs in settings:
```
http://localhost:5000
http://localhost:5000/callback
```
Now replace `CLIENT_ID` and `CLIENT_SECRET` in `index.js` with your application's client ID and client secret from your Spotify dashboard. Finally, replace `REDIRECT_URI` with `http://localhost:5000/callback`.
