# Spotify web API application

Node.js and Express js web app with Spotify web API functionality. Implements Authorization Code OAuth authentication flow, referenced from [this repo](https://github.com/spotify/web-api-auth-examples).

Here are steps for running a Spotify web app locally starting from this repo (requires [Node.js](https://nodejs.org/en/)):

## Setting up locally:
```
$ git clone https://github.com/tommygeiger/spotify-webapi    # or fork then clone
$ cd spotify-webapi
$ npm install
$ npm start
```
Your app should be up and running at localhost:5000 (but it's not going to work yet)

## Setting up a Spotify Web App:

You'll need to register a Spotify app and get your own credentials from the [Spotify for Developers Dashboard](https://developer.spotify.com/dashboard).

To do so, go to the [Spotify for Developers Dashboard](https://developer.spotify.com/dashboard) and create an application. Register these URIs:

http://localhost:5000

http://localhost:5000/callback

Now create a file in your `spotify-webapi` directory called `config.js` containing your Spotify app's client_id, client_secret and redirect_uri:
```
var config = {
  CLIENT_ID : 'your-spotify-app-client-id',
  CLIENT_SECRET : 'your-spotify-app-client-secret',
  REDIRECT_URI : 'your-redirect-uri' #i.e. http://localhost:5000/callback
}
```
