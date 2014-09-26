# Autolander

Autolander is a tool which manages continuous integration workflows between Bugzilla and Github.

## Development

Ensure that the :autolander (https://github.com/autolander) github account has push access to your repository.

Using ngrok for a tunnel to localhost is the easiest way to develop. Fork your repository of choice. Once you have a tunnel setup, add a webhook to your repository that points to https://<id>.ngrok.com/github.

```
./ngrok 80
```

Start the server.
```
node ./bin/app
```

## TODO
* Handle when a github merge fails.
* Store bugs we're interested in somewhere so we don't have to process *every* bug.
* Write end-to-end integration tets.