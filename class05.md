### Class 05 Reading

## Heroku

Heroku usese its own command line interface for managing and scaling apps, adding on, accessing app logs, and locally running the app. Installing the CLI allows a new series of heroku commands to function in terminal.

Heroku uses a create command which makes a git remote under the name *heroku* -- it is also locally associated. Pushing to the heroku remote works the same way as pushing to git, only it subs *heroku push origin master* for example instead of *git push origin master*.

Heroku keeps timestamped logs in one channel, which are aggregated from the output of both the app and its compoenents. These are accessed by the *heroku logs* command.