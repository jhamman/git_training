git_training
============

# Getting Start With Git #

[Introduction To Git Presentation](https://github.com/UW-Hydro/git_training/raw/master/presentation/GitIntro_jhamman.pdf)

The best way learn git is to use it. If you've never used git before, I recomend begining with this short, interactive tutorial: [Try Git](http://try.github.com/)

Now that you have some idea of what the commands are and the basic workflow, let's do some real world examples.  

## First some setup

**Local Configuration**

There are alot of configuration options in git.  The basics are listed below but you'll find you probably want to add more.  
 -- [Link to Configuration Options](http://git-scm.com/book/en/Customizing-Git-Git-Configuration)

    git config --global user.name my name”
    git config --global user.email “my_email@hydro.washington.edu”

**Setup a Github Account**

Github is a hosting service for git repositories.  Even if you don't use github as your standard remote, I reccomend setting up an account.  [Sign Up For Github](https://github.com/join) 

## Practice
Our practice will follow the [Github Bootcamp](https://help.github.com/categories/54/articles), with a few modifications.  

1. [Setup Git](https://help.github.com/articles/set-up-git) 

    If you are using your hydro computer, git is already installed (/usr/bin/git) and we've already taken care of the basic configuration, so you can skip to #2.  If you are on another machine, installation is pretty easy and is outlined in the link above.  

2. [Create A Repo](https://help.github.com/articles/create-a-repo)

    Everyone needs a "Hello-World" repository.  Follow the steps in the Create A Repo tutorial to create your own "Hello-World".

    *Bonus:  Now that you have that dialed, try repeating those steps for a project you've been working on.* 

3. [Fork A Repo](https://help.github.com/articles/fork-a-repo)

    Follow the steps in the tutorial to fork and clone the [Spoon-Knife](https://github.com/octocat/Spoon-Knife) repo.

    ####The assignment
    
    a.  Fork the [git_traning](https://github.com/UW-Hydro/git_training), [VIC](https://github.com/UW-Hydro/VIC), and [DHSVM](https://github.com/UW-Hydro/DHSVM) repositories.   

    b.  Now clone the your fork of the git_training repository to your local machine. i.e.: 
        
          git clone git@github.com:jhamman/git_training.git

       *Note: If you get an ssh error when you try to clone or fetch, check out Github's tutorial on [how to setup ssh keys](https://help.github.com/articles/generating-ssh-keys).*

    c.  Create a branch your local copy of the repo, something like
    
          git branch joes-example-branch

    d.  Checkout your branch
        
          git checkout joes-example-branch

      *Note: c and d can be done as a single step as* 
      
          git checkout -b joes-example-branch

    e.  Add a file to your repo (i.e. my_new_file.txt).  The commands you'll need for this are:

        touch my_new_file.txt
        git add
        git commit # Don't for get a good commit message

    f.  Push your changes to your Github fork.
        
        git push origin joes-example-branch

    e.  Submit a pull request to UW-Hydro.  This is done from your Github Repository Page.

4. [Be Social](https://help.github.com/articles/be-social)

    Not mandatory but you can follow an organization (i.e. [UW-Hydro]()) or a person (i.e. [Joe Hamman](https://github.com/jhamman) if you want to stay tuned to ongoing developments on github
5. [GitHub Glossary](https://help.github.com/articles/github-glossary)

References and Links:

- [git-scm](http://git-scm.com/) - Git's home page
- [Github](https://github.com/) - Github home page
- [Git-Flow](http://nvie.com/posts/a-successful-git-branching-model/) - This is the branching model and workflow that VIC and DHSVM and a good way to think about how branching can help you work more effeciently.  
