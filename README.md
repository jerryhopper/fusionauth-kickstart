# fusionauth-kickstart


### What is Kickstart?

Kickstart is the name of FusionAuth's template-system for quickly setting up a fusionauth instance. Kickstart allows you to build a template that will be executed during startup to quickly replicate development or production environments. No clue what fusionauth is?  Checkout https://fusionauth.io

### What is Github Actions?

GitHub Actions is an API for cause and effect on GitHub: orchestrate any workflow, based on any event, while GitHub manages the execution, provides rich feedback, and secures every step along the way. With GitHub Actions, workflows and steps are just code in a repository, so you can create, share, reuse, and fork your software development practices. Read all about it here : https://github.com/features/actions 


### About this repo
In this repo, i demonstrate the how to use Fusionauth's kickstart.json to quickly setup a fusionauth instance with a preconfigured application with specific grants and a user so we can test some code against fusionauth.

To keep things simple, the code that is being used is a simple device-authorization script in bash (source: https://raw.githubusercontent.com/jerryhopper/fusionauth-bash-deviceauth)

More info about device authorization : https://fusionauth.io/learn/expert-advice/oauth/oauth-device-authorization/

### How to use this repo?

This repository is here to help you create tests for your own code, and because you need to push a change to trigger the github-actions, you need to clone this repository and push a change. This will trigger a action as defined in /.github/workflows/test.yml 

Now you can see the progress of the action in the 'actions' tab of your git-repository.

If everything goes well, all tests will succeed. (https://github.com/jerryhopper/fusionauth-kickstart/actions/runs/400985304)


### What's next?

Now you can test your own custom code against a pre-configured fusionauth instance, without the need for a development enviroment.

If you are interested how you can do this in conjunction with travis CI, checkout this repo : https://raw.githubusercontent.com/jerryhopper/fusionauth-bash-deviceauth
