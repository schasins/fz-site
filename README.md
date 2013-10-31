fz-site
=======

Getting set up:

Clone this repo.  At the command line, navigate to the folder where you want to store your website.  Run this command:

```
git clone 'https://github.com/schasins/fz-site.git'
```

Add your heroku repo as a remote.  Navigate into your fz-site folder (that is, into your repo), then run this command:

```
git remote add heroku 'git@heroku.com:<repo_name>.git'
```

Normal editing:

Inside your repo, navigate to the public directory.  You can put your pages here.  You can start by modifying the index.html page that's in there right now!

If you make a new file, make sure to run this command:

```
git add <new_file_name>
```

This adds the file to your repository so that github will track it, and so that it will get pushed to the server when you deploy the site.

If you've made some changes that you're happy with, and that you want to be able to look back at later, run this command:

```
git commit -am "<here say something descriptive about the changes you've made since the last commit>"
```

This version of the command just commits all the changes you've made to tracked files in the repo.  If you want to do something more specific like just committing a single file's changes, you could do:

```
git commit <file_name> -m "<here say something descriptive about the changes you've made since the last commit>"
```

Once you've committed changes, you can push the changes to github so that you have the files backed up on github's servers.  To do that, you use this command:

```
git push origin master
```

This backs up your changes to github so you can look at them on the github site, but it doesn't change what heroku is serving, and since heroku is the one that's actually serving your site on the web, you have to change heroku's version of your repo to actually deploy a new version of your site.  When you're ready to deploy a new version, run this command:

```
git push heroku master
```

If you have any questions, just ask me!
