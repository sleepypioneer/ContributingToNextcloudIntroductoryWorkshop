<a name="top"></a>
# :computer: Contributing To Nextcloud Introductory Workshop

![Nextcloud](https://github.com/sleepypioneer/ContributingToNextcloudIntroductoryWorkshop/blob/master/images/nextcloud%20conf.jpeg)

Interested in contributing to Nextcloud but not sure how? In this introductory workshop we will guide you in getting your development environment set up and starting your pull request.

This workshop is being run with support from [Open Source Diversity](https://opensourcediversity.org/#), a monthly Meetup group in Berlin that provides a friendly and safe environment for contributing to open source. 

We look forward to getting you started with contributing to Nextcloud Open Source software!

***

# :cloud: Nextcloud :cloud:
Nextcloud at it's core is a open source self hosted file sharing software but it also offers a lot more. With additional apps you can not only manage your data but interact with it in a collaborative and creative manner with upmost privacy & security!

You can learn more about Nextcloud including how to install it and where to get self hosting on their website : https://nextcloud.com/

***
[Back to Top](#top) 
# :woman: Contribute :man:

*"Contributing to open source can be a rewarding way to learn, teach, and build experience in just about any skill you can imagine."* ~
https://opensource.guide/how-to-contribute/

An open source project is all about its contributors. Over 1000 people have code in Nextcloud. About a 10th of those have direct access to the code in the repository, contributing regularly. Besides coders, there are designers, Nextcloud advocates, translators, forum admins and many others who are part of the community.

With so many ways to get involved, what are you waiting for :smile:

### Ways to contribute to Nextcloud
* [Develop your own App](https://docs.nextcloud.com/server/14/developer_manual/app/)
* Improve existing Nextcloud code *(if you're new to software development, good first issues are a good place to start)*
* [Review new code](https://nextcloud.com/blog/get-involved-in-nextcloud-by-reviewing-pulls/)
* Help with translations
* Help with the Design *(go to the [design page](https://nextcloud.com/contribute/design/))*
* Test the software
*(Testing upcoming Nextcloud Server releases is the best way of making sure the new release can do what you need it to do. And of course, only if you report a problem to us we know about it and can fix it! If you have a bug to report, find the [issue submission page.](https://github.com/nextcloud/server/blob/master/CONTRIBUTING.md))*

You can show publically on your Github account that you contribute to Nextcloud by setting yourself as public in the [GitHub organization](https://github.com/orgs/nextcloud/people)

For more details about contributing to Nextcloud visit : https://nextcloud.com/contribute/

***
[Back to Top](#top) 

# :pen: Tools you will need

You will also need a few other useful tools to contribute which we will cover here.

* [IRC communication Tool](#irc)
* [Git with a github account](#github)
* [IDE /Text editor (Visual studio Code - open source)](#ide)
* [Nextcloud Docs](#docs)


<a name="irc"></a>
### :loudspeaker: IRC Chat

On IRC you can connect to other contributors and ask questions. You can also help others with their code.

There are a few chat tools you can use we reccomend [Riot](https://about.riot.im/)

You'll need to register your username first in order to use our channels. You can find instructions here:  https://gist.github.com/fstab/ce805d3001600ac147b79d413668770d

You can then access the Nextcloud developers room through this link:
https://riot.im/app/#/room/#freenode_#nextcloud-dev:matrix.org

<a name="github"></a>
### :octocat: Github & Github Desktop

In order to contribute to the code base and checkout the latest versions you will need to make a free github account, if you don't already have one you can sign up [here](https://github.com)

https://github.com/nextcloud

Commands to download and upload code can be done through the terminal *(on windows you will also need to [install git](https://git-scm.com/downloads))*

Alternatively you can use the Github Desktop GUI which you can download [here](https://desktop.github.com/) *(we can highly reccomend this for complete beginners to Git)*

<a name="ide"></a>
### :gem: IDE / Text Editor

To work on the code base you will need a IDE or Text Editor. 
Here the choice is completely yours and it is a personal preference which you find best to work with. However, we can highly recommend Visual Studio Code. Below are also some others you may like to try (they are all free).

<a name="docs"></a>
### :blue_book: Nextcloud Documentation
Nextcloud already has a vast amount of documentation for getting started, style guides and about how the code base is structured. You need to make sure you are working within these guidelines when you are fixing issues so it is very useful to keep them at hand!

https://docs.nextcloud.com/server/14/developer_manual/

This also includes their code of conduct, if you encounter behaviour aimed at yourself or other that goes against this code do not be afraid to report it! https://docs.nextcloud.com/server/14/developer_manual/general/code-of-conduct.html

***
[Back to Top](#top) 

# :memo: Running the Nextcloud development environment

You'll need to set up your development environment to test and program on the Nextcloud codebase. The following guides are to get you started depending on which OS you are using. For Mac and Linux you can run this natively on your machine, for Windows you will have to install a Virtual Machine or for all three you can use the Docker setup we have prepared to run the environment in a isolated container.

For this workshop we reccomend working with Docker so please follow the official set up guide to install Docker on your machine.

:whale: https://www.docker.com/get-started :whale:

We will take time to go through these guides with you shortly as each set up can be a little different and challenging. (We've all been there at some point :wink: .)

* [Mac](https://github.com/sleepypioneer/ContributingToNextcloudIntroductoryWorkshop/blob/jessica/setupGuides/NextcloudMacDevelopmentEnvironment.md)
* [Linux (with Docker)](https://github.com/David-Development/nextcloud-dev-docker/blob/master/README.md)
* Windows [with Docker](https://github.com/David-Development/nextcloud-dev-docker/blob/master/README.md)
          [or with a VM](https://github.com/sleepypioneer/ContributingToNextcloudIntroductoryWorkshop/blob/jessica/setupGuides/NextcloudWindowsDevelopmentEnvironment.md)
          
Big thanks to @jancborchardt & @David-Development for their support in creating these documents

***
[Back to Top](#top) 


If you didn't follow the Docker guide you will still need to get the code, here is a quick guide to doing so with Github either in the Terminal or through github Desktop.

## :1234: Through the Terminal

### Cloning a Repo to your machine

To start working on an issue or a feature for a repository (nextcloud server or one of the app for example) you will need to download (clone) the project to your local setup.

`git clone https://github.com/nextcloud/server`

### Forking a Repo

Usually you don't have permissions to a repository that does not belong to you. To allow you to edit the code, you can *fork* the repository to your own account. That means you can clone the project and start coding on your account.

![forkbutton](https://github.com/sleepypioneer/ContributingToNextcloudIntroductoryWorkshop/blob/master/images/forkbutton.png)

After that just make your changes directly to your own forked repository and you will be able to create a pull request to the original project afterwise.

### Creating your own Branch

On your local clone, you will need to create a new branch to start adding your modifications. Just checkout the branch you want to edit (usually master)

`git checkout master`

and then create a new branch based on the one we just selected.

`git checkout -B your-branch-name`

***
[Back to Top](#top) 

## :octocat: Through the Github Desktop client

`Go to clone `

<img src="https://github.com/sleepypioneer/ContributingToNextcloudIntroductoryWorkshop/blob/master/images/GitHubDesktopSetup1.PNG" alt="drawing" width="400"/>

<img src="https://github.com/sleepypioneer/ContributingToNextcloudIntroductoryWorkshop/blob/master/images/GitHubDesktopSetup2.PNG" alt="drawing" width="400"/>

`Respositories > Open in visual studio code`

Changes made to the code will appear in the right hand side of the Desktop client

<img src="https://github.com/sleepypioneer/ContributingToNextcloudIntroductoryWorkshop/blob/master/images/GitHubDesktopSetup3.PNG"/>

You can create your own branch and publish it to the repo

<img src="https://github.com/sleepypioneer/ContributingToNextcloudIntroductoryWorkshop/blob/master/images/GitHubDesktopSetup45.PNG" alt="drawing" width="600"/>

You can add a commit message and push your commit to the chosen branch.

<img src="https://github.com/sleepypioneer/ContributingToNextcloudIntroductoryWorkshop/blob/master/images/GitHubDesktopSetup6.PNG" alt="drawing" width="600"/>

[Back to Top](#top) 


:apple: Now we will take time to make sure you have everything set up and take a short break. Afterwards, we will go to [part 2](https://github.com/sleepypioneer/ContributingToNextcloudIntroductoryWorkshop/blob/master/partII.md).
