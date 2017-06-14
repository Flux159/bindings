# Official bindings for µWebSockets
* Node.js binding lives here, report issues with µWS itself over at uWebSockets repo. Report issues with the Node.js binding here.
* Create new bindings and get them merged here.

# Deployment Workflow: 
Travis CI and Appveyor CI are setup for automatic continuous integration testing on commit. Publishing to NPM is also setup automatically on new tagged version.

```shell
git push # Push changes to master, CI runs automatically, make sure it works & passes all tests by checking Travis CI and Appveyor
git tag -a v0.20.0 -m 'Version 0.20.0' # Create new tag
git push --tags # Push tags independently after push to master, CI and deploy runs automatically
```
