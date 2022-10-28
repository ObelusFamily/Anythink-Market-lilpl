# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

At Anythink, our engineers work with a development environment that's hosted in the cloud called Github Codespace. No need to install anything on your own computer!

It takes about a minute to boot. Once it's up and ready you can start working directly in the browser or use VS Code to connect to the codespace in the cloud.

Go ahead and clone this repository first, before doing any other setup. Clone it, don't fork it!

[Create your CodeSpace](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=558990617)
Note: No need to change anything in the default options, just click on the Create codespace button and wait for it to boot

Once your codespace is up and running you can now run `docker-compose up` in your codespace's terminal to load Anythink's backend and frontend.

Once docker-compose finishes loading up, the backend should be running and able to connect to the database.

After the server is up, make sure you test it by pointing your browser to https://<your domain>.githubpreview.dev/api/ping
You should get back a response: `{"msg":"Pong! Seems like Everythink is working, great job!"}`

Check the frontend and make sure it’s connected to the backend.
If everything is working properly, you’ll be able to create a new user on https://<your domain>.githubpreview.dev/register