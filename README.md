# fusionauth-kickstart


### What is Kickstart?

Kickstart is the name of FusionAuth's template-system for quickly setting up a fusionauth instance. Kickstart allows you to build a template that will be executed during startup to quickly replicate development or production environments.

### What is Github Actions?

GitHub Actions is an API for cause and effect on GitHub: orchestrate any workflow, based on any event, while GitHub manages the execution, provides rich feedback, and secures every step along the way. With GitHub Actions, workflows and steps are just code in a repository, so you can create, share, reuse, and fork your software development practices. 


In this repo, i demonstrate the how to use Fusionauth's kickstart.json to quickly setup a fusionauth instance with a preconfigured application with specific grants and a user so we can test some code against fusionauth.

To keep things simple, the code that is being used is a simple device-auth script in bash (source: https://raw.githubusercontent.com/jerryhopper/fusionauth-bash-deviceauth)


### How to use this repo?

This repository is here to help you create tests for your own code, and because the github-actions log is not visible to non-owners you need to clone this repository, and push a change. This will trigger a action as defined in /.github/workflows/test.yml 

Now you can see the progress of the action in the 'actions' tab of your git-repository.

If everything goes well, all tests will succeed.


### What's next?

Now you can test your own custom code against a pre-configured fusionauth instance, without the need for a development enviroment.

If you are interested how you can do this in conjunction with travis CI, checkout this repo : https://raw.githubusercontent.com/jerryhopper/fusionauth-bash-deviceauth
