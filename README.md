# fastai-binder-app-template
A template github project for building your binder app based on [Lesson 3 of the fastai course v4](https://course.fast.ai/videos/?lesson=3) (2020) and also discussed in [Chapter 2](https://github.com/fastai/fastbook/blob/master/02_production.ipynb) of the book "Deep Learning for Coders with fastai and Pytorch" . This template is based on the [instructions posted on the fastai forums here](https://forums.fast.ai/t/deploying-your-notebook-as-an-app-under-10-minutes/70621?u=butchland).

## Instructions for Deploying to Binder

_Do the next step only after making sure your voila app is running_
1. Create a github account if you don't have one yet.
1. Clone this repo as a template for your own binder app repository. 
    * If you are running on a jupyter notebook, you can create a terminal to run your git clone commands.
    * If git is not installed on your jupyter environment, install it by following [these instructions](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
    * You might have to run the following commands to setup your email and username for git:
        * `git config --global user.name "<Your name>"`
        * `git config --global user.email "<email@address>"`
    * In order to push code to a github repo, it is usually convenient to create an ssh key to authenticate yourself. See [instructions here](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh) on creating an ssh key and registering it on github.
1. Copy over the following:
    * the `export.pkl` created in [Chapter 2](https://github.com/fastai/fastbook/blob/master/02_production.ipynb) as the exported learner for classifying bear images
    * the `requirements.txt` located in the [fastbook](https://github.com/fastai/fastbook) directory 
    * the stripped down notebook containing the voila app only. A [sample notebook](https://github.com/butchland/fastai-binder-app-template/blob/master/sample-fastai-binder-app.ipynb) is provided but stripping down the [Chapter 2 notebook](https://github.com/fastai/fastbook/blob/master/02_production.ipynb) is a good exercise.
1. Test your stripped down voila app notebook using voila in your jupyter environment.
1. Install `git lfs` on your local environment. If you are running on Jupyter notebook, create a terminal and run your installation commands there.  See [instructions here](https://github.com/git-lfs/git-lfs/wiki/Installation)
1. Push your code changes into your github repository. Run the following git commands:
    * `git add .`
    * `git commit -m 'Add my app notebook and exported learner'`
    * `git push`
1. Follow the [instructions to run the app on binder](https://forums.fast.ai/t/deploying-your-notebook-as-an-app-under-10-minutes/70621?u=butchland). _Note that the `.gitattributes` file has already been provided as part of this template repo_

 
