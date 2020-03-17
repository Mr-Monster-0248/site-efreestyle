# Site Web Efreestyle
![build icon](https://github.com/Mr-Monster-0248/site-efreestyle/workflows/Jekyll%20build%20site%20CI/badge.svg)
![Publish website](https://github.com/Mr-Monster-0248/site-efreestyle/workflows/Publish%20website/badge.svg)

This is the devellopent repository for the efreestyle webiste

## Prerequisite
As this project is a jekyll based website you will need all the software to build a jekyll website.

You will find everything in the [Jekyll documentation](https://jekyllrb.com/docs/)

## Building project
### While developing
The jekyll tools provides a commande to run a local server to test the website. `bundle exec jekyll serve`. You can uses this commande to develop and test the website **before** commiting any changes to the master branche

If any error please refer to the [Jekyll documentation](https://jekyllrb.com/docs/)

### Before any push to the master branche
Make sure the commande `bundle exec jekyll build` pass correctly. The github actions are here to prevent any unbuilding push but it is still a good habit to have.

## CI/CD with Github action
The porject uses Github action to **build** and **upload** the website to a Qithub page
- For heach push to the master branch the build action check if the project build correctly
- Once the build pass and you wat to upload the new website to github page make a release in Github, an action will take care of the deployement
