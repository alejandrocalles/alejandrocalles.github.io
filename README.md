# Portfolio

🚧 This site is currently under construction 🚧

## Running locally

To run locally, use the following command

```bash
bundle exec jekyll serve
```

To enable live reload of changes made to the website files, use the
`--livereload` option:

```bash
bundle exec jekyll serve --livereload
```

To show any posts in the `_drafts` folder, use

```bash
bundle exec jekyll serve --draft
```

## Note on minima

This project depends on version 2.5.1 of minima.
This is specified by this line of the Gemfile

```
gem "minima", github "jekyll/minima", ref: "..."
```

where the `ref` is the latest commit of the `2.5.1` tag.

The "reason" for this dependecy is that the `_includes/home.html` file
in this project is a modified version of the file in that specific
version of `minima`, so this is not a hard dependency, but
using a different version might break things.
