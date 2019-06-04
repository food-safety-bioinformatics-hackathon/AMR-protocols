# How to contribute to this project

This is an open documentation project and we welcome all contributions.


## Contributor Agreement

By contributing, you agree that we may redistribute your work under the license that this project uses. In return, you will be recognized as a contributor to this project, which will be reflected in the [authors](authors.md) document in this repo. We expect all contributors to abide by the project’s code of conduct. 


## How to contribute

The easiest way to get started is to file an issue to tell us about a spelling mistake, some awkward wording, or a factual error. If you do not have a GitHub account, you can send us comments by email. However, we will be able to respond more quickly if you use one of the other methods described below.

If you have a GitHub account, or are willing to create one, but do not know how to use Git, you can report problems or suggest improvements by creating an issue. This allows us to assign the item to someone and to respond to it in a threaded discussion.

If you are comfortable with Git, and would like to add or change material, you can submit a pull request (PR). Instructions for doing this are included below.


## What to contribute

We are very happy to receive any and all contributions regarding the subject matter of this resource in whichever manner you are able to submit them. Many different things can be contributed, you can send us an email about relevant reports, you can submit an issue informing us about an error you found, or you can submit a pull request contributing text on a new method or a procedure. 

If you would like to contribute, and don’t know quite where to start or what to do, please check the list of current issues for the repository. 


## Using Github

If you choose to contribute via GitHub, you may want to look at How to Contribute to an Open Source Project on GitHub. 
The current version of this resource is to be found in the master branch. This branch stays static until we decide that we have a new release. All development happens on the **dev-branch**. If you want to contribute, we request that you work on that one.  

How to proceed:
  * Fork (i.e. copy) the project to your account
  * Go to your fork, and change the branch of the project to the current development branch 
  * Then add/modify the contents you want. This can be done directly in your fork on github
  * Commit the change
  * Send your pull request
  * Your pull request will be merged dev-branch after manual checking
  * The admins will then rebuild the dev-branch
  * The dev-branch will be merged to master repository with the next release


## Adding your protocol to the site

To add a protocol, please fork or clone this repository, add your procotol and then submit a pull request. You can add more than one protocol at a time.

For example:

* download the current repository
```bash
git clone https://github.com/food-safety-bioinformatics-hackathon/AMR-protocols

cd AMR-protocols

git checkout master

git pull origin master
```

* checkout a new branch for your protocol
```bash
git checkout -b newProtocol
```

* write a new protocol (see the next section below for a guide)
```bash
cp template docs/_posts/2019-06-01-newProtocol.md
vim docs/_posts/2019-06-01-newProtocol.md
```

*  push the protocol to the repository
```bash
git add .
git commit -m 'adding my new protocol'
git push -u origin newProtocol
```

* go to the [repo on github](https://github.com/food-safety-bioinformatics-hackathon/AMR-protocols) and create a new pull request so that we know to merge in your protocol into the master branch.


The web site for this project is generated using [Jekyll](https://jekyllrb.com/). When a pull request is accepted, your protocol will be merged into the github repository master branch and it should then trigger the site to re-build with your new content.


## Writing a protocol

Please use the [template](template.md) to structure your protocol. In terms of the top few lines, please make sure you put in your own values for the following:

*date
*title
*categories
*description
*doi

It is important that you follow the same date convention. Please also make sure that your title is unique.

Once you have edited the top few lines of metadata, you can write your protocol. Please use [markdown format](https://guides.github.com/features/mastering-markdown/) and add your content from `Summary` onwards. If you can, please use our suggested headings.

Store your protocol in `docs/_posts`. Make sure you save it using the filename convention (`YYYY-MM-DD-tag.md`).

Check the FAQ of the website or ask us a question if you need help!
