# github.io

You can create and publish GitHub Pages online using the Automatic Page Generator. 
If you prefer to work locally, you can use the GitHub for Mac and Windows apps, or the command line.

User & Organization Pages

User & Organization Pages live in a special repository dedicated to GitHub Pages files. You will need to name this repository with the account name, e.g. atmos/atmos.github.io

    You must use the username.github.io naming scheme.
    Content from the master branch will be used to build and publish your GitHub Pages site.

You can only use your own account name for a User or Organization Page repository. A repository like joe/bob.github.io will not build a User Pages site.

When User Pages are built, they are available at http(s)://<username>.github.io.


$ git clone https://github.com/user/repository.git
$ cd repository
$ git checkout --orphan gh-pages
$ echo "My Page" > index.html
$ git add index.html
$ git commit -a -m "First pages commit"
$ git push origin gh-pages
