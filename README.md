New Project
===

To rapidly prototype a new concept as a static site, I typically reuse a number
of base files and styles, which frees me from reimplementing or reconsidering
stylistic decisions and allows me to focus on the logic.  To do so, I use a
simple bash script which generates a lot of the boilerplate from template files.

After cloning the repo, I copy the executable and the templates into my path,
e.g.:

```
$ git clone https://github.com/NathanielWroblewski/new-project.git
$ cd new-project
$ cp new-project ~/bin/new-project
$ chmod u+x ~/bin/new-project
$ cp -r templates ~/bin/templates
```

Then, I can bootstrap a new project via:
```
$ new-project my_project_name
```

The script makes a number of simplifying assumptions, one of which is that projects live within `~/Desktop/side/`.
