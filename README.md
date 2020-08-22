# DISPATCHES website

This is the DISPATCHES project website, hosted on Github at 
https://gmlc-dispatches.github.io

## Developer instructions

If you are modifying the website, follow these instructions.

### Installation

1. Clone or download the repository
2. Change to the directory of the repository
3. Install required Python modules: `pip install -r requirements.txt`
4. Build/serve website (see below)

### Building the website

The website is built using [MkDocs](https://www.mkdocs.org).
To rebuild the website, follow the standard procedure for this
static site generator:
```
# generate static files in 'docs'
mkdocs build
# preview the website on the local host
mkdocs serve
```

Once you start the server, you can make changes to the 
configuration, 'mkdocs.yml' or the Markdown source
files in 'src/', and the changes will be reflected immediately
in the local webpage (by default, at `http://127.0.0.1:8000`).

### Pushing changes to the web

The following assumes you are working in a clone of the 
[main repository](https://github.com/gmlc-dispatches/gmlc-dispatches.github.io).
You can also work in your fork and submit pull requests.

To commit the changes you made locally add/commit with git both
the files in the 'src' directory *and* the files that were added
with the `mkdocs build` command in the 'docs' directory.
The simple way to do this is just to add all new files and commit
in one command: `git commit -am "my change message"`.

Once you have committed your changes locally, `git push` up to the
master branch. After several minutes, your changes should show up
in the public website.
