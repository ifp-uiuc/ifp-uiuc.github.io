# The IFP website, made using Jekyll.
This site is designed to make it easy to add small updates. If you want to add new memebers, old members, projects, and publications, it just involves updating the right yaml file, and putting images in the right directory.

If you want to make larger changes to the site, it will require more work.

# Updating the site
To update the site, you will need some familiarity with git. If you don't, brush up first.

First, you need to clone it:

```
git clone git@github.com:ifp-uiuc/ifp-uiuc.github.io.git
```

If you have already cloned the repo, make sure your copy of the repo is up-to-date:

```
git pull origin master
```

Next make changes to the files. Once you are done: add, commit, and push the changes:

```
git add .
git commit -m 'Description.'
git push origin master
```

## Small updates

### Memebers
To add a new member, edit `./_data/members.yml`. Add a new entry at the end of the file in the form:

```
- name: Shiyu Chang
  image: shiyu.jpg
  text:
  social:
    - title: envelope #use for email address
      url: mailto:chang87@illinois.edu
    - title: link
      url: http://www.ifp.illinois.edu/~chang87/
```

Then move the picture into `./assets/img/members`.

When you are done: add, commit, and push the changes.

### Past Members
To add a past memeber, edit `./_data/past_members.yml`. Add a new entry at the end of the file in the form:

```
- name: Ashutosh Garg
  job: Bloomreach Inc.
  email: ashutosh@ifp.uiuc.edu
  url: http://www.ifp.illinois.edu/~ashutosh/
```

When you are done: add, commit, and push the changes.


### Projects
To add a new project, edit `./_data/projects.yml`. Add a new entry at the end of the file in the form:

```
- name: Project Name
  image: project-figure-name.png
  text: 'Description.'
```

Then move the picture into `./assets/img/projects`.

When you are done: add, commit, and push the changes.

### Publications
To add a publication, edit `./data/publications.yml`. Find the appropriate section (e.g. Books, Book Chapters, Journal Papers, etc), and add a new line under articles. For example:

```
  - "A. Author, T. Huang, Paper Title, Conference Name, 2016."
```

When you are done: add, commit, and push the changes.
