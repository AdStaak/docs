## Form Tools Documentation

This repo contains the Form Tools documentation for the upcoming Form Tools site, to be found at docs.formtools.org. It 
includes all documentation: the main userdoc, installation, upgrading instructions, module documentation and API.

We use [Jekyll](http://jekyllrb.com/) to handle generating the actual markup. Jekyll is a *static website generator*. 
In other words, rather than the web pages being constructed on the fly as people request them from the server, all the 
heavy lifting is done beforehand. The site is *generated* before being pushed to the server. 

The new website + docs have lots of benefits:
- **Speed!** - static files are far faster to load than the PHP/MySQL-heavy website right now. 
- **Open!** - now that the doc is in a public repo, it's super easy for people to contribute and fix documentation,
unlike the old site where the doc is in a closed database.
- **more secure** - the old Form Tools site has a whole bunch of different pieces of software running on it, 
and it's been hacked more than once.


## Contributing

Fixes to the documentation and contributions are always welcome! You can contribute in two ways:

1. Browse the documentation online and click the "EDIT PAGE" button when you find an error, or something you'd like to
improve on. That will take you to github.com where you can edit the page right through your web browser.

2. Clone the repository and build it locally. There, make your changes and submit a *pull request*. You might want to 
do this if you want to contribute a new tutorial, for example.

I manually review all contributions.


### How to build locally

If you want to run the documentation locally, you'll need to do the following:

1. Clone this repo.
2. Install Jekyll via the [instructions here](http://jekyllrb.com/docs/installation/)
3. Once it's been installed, open up your terminal/command line, navigate to the root folder of this repo and enter:
```
npm install 
npm install -g grunt-cli
```

4. Next, start up the doc with `grunt start` (I need to run `sudo grunt start` myself).

That starts a local server which you can access at `http://localhost:4000/docs/`. At this point, you can edit the files
locally and the HTML files will be automatically regenerated on the fly.


### Remaining TODO (for me)

- remove all tables 
- search for 'demo' and remove any references
- link checker on the entire doc (once complete)
- search for 'feature suggestions' & make sure they're linking to github
