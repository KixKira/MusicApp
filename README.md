# MusicApp

To get the beta version of the application working, you must do the following:

* You must enter your Spotify as a developer: https://developer.spotify.com/
* You go to Dashboard
* Log In
* You choose the application, if you don't have any, you create it
* Show Client Secret
* You will have the Client ID and the Secret ID
* You go to the Postman
* You create a new Request of type POST
* Paste the following URL: https://accounts.spotify.com/api/token
* Body tab
* Select: x-www-form-urlencoded
* The KEY values will be: grant_type, client_id, client_secret
* The VALUE values will be: client_credentials, your client_id and client_secret generated in Spotify
* Click on SEND
* Will generate the following: {
    "access_token": "TOKEN",
    "token_type": "Bearer",
    "expires_in": 3600
}
* On the page spotify.servise.ts, line 18, next to Bearer, paste the access_token
* And voila, it will work for 1 hour

Any questions, feel free to write to me.
