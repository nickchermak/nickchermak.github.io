Make sure login into nickchermak github and github desktop

USE GIT BASH

verify with: 
$ git config --global user.name
$ git config --global user.email

clone repo

run:
bundle install
bundle add jekyll-seo-tag
bundle install
bundle exec jekyll serve  #this will push to local server

if get java error run:
export PATH=$PATH:/c/Users/nickc/AppData/Local/Packages/PythonSoftwareFoundation.Python.3.11_qbz5n2kfra8p0/LocalCache/local-packages/Python311/Scripts

then run:
bundle exec jekyll serve

cancel local and run:
bin/deploy --user

make sure to us gh-pages and not main: 
git checkout gh-pages

git push origin gh-pages

might need to do this if forgot to set gh-pages:
git commit --allow-empty -m "Trigger GitHub Pages rebuild"
git push origin gh-pages



  
