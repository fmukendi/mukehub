
https://levelup.gitconnected.com/build-a-personal-website-with-github-pages-and-hugo-6c68592204c7

----- Git Hub pages trial  -----

hugo new site mukehub

cd mukehub

git init

git submodule add https://github.com/matcornic/hugo-theme-learn.git themes/hugo-theme-learn


➜  themes cd ..
➜  mukehub hugo new posts/my-first-post.md

Add to config.toml
baseURL = "https://fmukendi.github.io/"
languageCode = "en-us"
title = "My New Hugo Site"
# Change the default theme to be use when building the site with Hugo
theme = "hugo-theme-learn"

///hugo server -D
hugo server
////hugo server -t hugo-theme-learn

hugo     // to create public folder 
---------------------------------------------

Create repo to hold github pages

echo "# fmukendi.github.io" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/fmukendi/fmukendi.github.io.git
git push -u origin master
----------------------------------------------
cd public
git init
git add .
git remote add origin https://github.com/fmukendi/fmukendi.github.io.git
git commit -m "first commit"
git push origin master

  or 
git submodule add -b master git@github.com:fmukendi/fmukendi.github.io.git public

cd public

git add .

git commit -m "push"

git push origin master