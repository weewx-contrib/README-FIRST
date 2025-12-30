## weewx-contrib
This github organization was created to let developers 'optionally' host or duplicate their github repos in a central place for people to more easily find.

### What is a Github Organization

Github organizations permit a setup where a defined set of users can essentially contribute collectively, with some level of access control and overall control.

It seems that the aggregate size is limited to 500 MB, so we do need to set some limits....

#### Rules of the Road

1. Be nice.  Be polite.  Do not offend.  All the things you're taught at 2 years old apply.
2. When in doubt, consult rule (1) above.
3. Github users must specifically ask to be made a 'member' of this github organization **_(how to do so is TBD)_**
4. It might take a day or so for an admin to have time to add you.  Be patient.  Consult rule (1) as needed.
5. Once an org admin has added you as a member, you will have the ability to create repos here.
6. All repos here must be 'public' only.  If you need a 'private' repo, please use your personal github account.
7. You may of course choose to work with other members as co-admins of 'your' repos.  Your repo is your turf.  You set the access rules for who can do more than read.

### What Kinds Of Repos Maybe Be Hosted Here

In short - anything that adds functionality ala the [official list](https://github.com/weewx/weewx/wiki#extensions-to-weewx) in the WeeWX Wiki.
* drivers
* extensions
* generators
* services
* skins
* uploaders

If you choose to host your repo here, please edit the official weewx wiki page to point here.

### What May Not Be Hosted Here

Anything else, including but not limited to:
* HOWTOs
* standalone build/install/configure scripts or the like
* anything like a blog or documentation-only set of pages

Bottom line is if it is a code addition to weewx, it's ok to consider hosting here.

### How To Upload Your Repo

#### Add your repo by importing it from your personal github
```
  Use the create new repository => import feature.
  Note that unfortunately this will not import your wiki
  It is uncertain if it will import your Issues

```

#### Add the repo here as another remote to your personal github repo
To quickly add your existing repo and push here as a remote named 'org'
```
  create the repo here via the repositories create button and menus
      please ensure that you've set it to be public

  # set it up as a git remote (this example names the remote 'org'
  git remote add org https://github.com/weewx-contrib/YOURREPONAME.git

  # check it is a remote
  git remote -v

  # push your repo's 'main' branch to the remote named 'org'
  git push -u org main
```
