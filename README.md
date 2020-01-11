# Jiggy's Site

A place to host all my internet facing sites.

## Mkdocs

The site is built using [MkDocs](http://www.mkdocs.org/).

Run the following command to install `python3`, `mkdocs` and mkdocs dependencies.

```sh
brew install python
pip3 install mkdocs markdown-include pygments mkdocs-material
```

To view the site locally:

```sh
mkdocs serve
```

A webserver will then be available at [http://127.0.0.1:8000](http://127.0.0.1:8000) to view your documentation.

Prior to uploading, run the markdown linter to ensure your formatting is correct, and ensure `mkdocs build` succeeds and include all generated files.

Building:

```sh
mdl .
```

```sh
mkdocs build
```

After successful mkdocs build, deploy changes from your forked repo:

**Note**: Only run the command below if you are on a forked repo.

```sh
mkdocs gh-deploy
```
