# My Current Code Log for #100 days of Code.
[My Current Progress](https://nerajno.github.io/100DaysOfCodeLog/log3.html)

This repo is being used to track my progress for  the 100 Days of Code Challenge ([https://100daysofcode.com](https://100daysofcode.com)) following Alexander Kallaway's examples.
This repo also uses the format of James Priest's ([repo](httpsgem install bundler
://github.com/james-priest/100-days-log)) to format this log, follow the instructions on his ReadMe if you want to use this format.

#### Todo {Current Round => Dec 20, 2023 to Mar 28, 2024 }
- [ ] Update Readme to standardize version.
- [ ] Implement personal branding and improve storytelling for the whole log.
- [x] Brainstorm this version and update accordingly.


## Current Mental Status
[![Groot looking ](https://media.giphy.com/media/B9XXtlIKF8wec/giphy.gif)](https://media.giphy.com/media/B9XXtlIKF8wec/giphy.gif)

#### Embedding Images in Log

Use this format to embed a **simple, non-clickable** image.

```bash
![image alt text](assets/images/my-file_small.jpg)
```

Use this format to embed a **clickable image** which displays a larger version on click.

```bash
[![image alt text](assets/images/my-file_small.jpg)](assets/images/my-file.jpg)
```

#### Log Customization

THIS SECTION IS A WIP... and still needs to be completed.

This is a list of items that can be customized at the top of each page.

- Header text
- Header description
- Header background color
- Page background color
- Link colour

These items can be customized for the site.

- Favicon - replace the icon in `docs/assets/images/icons/favicon.ico`
- Heading text for default page - `/_config.yml`

## Miscellaneous

#### Recommended Workflow

- VSCode extensions that I use for my log.
  - Code Spell Checker
  - Markdown All in Once
  - Markdown Emoji
  - Markdown Preview Git
  - markdownlint

<!--
1. Open folder
2. Start up site in terminal
3. Make changes
4. other... -->

### Under the Hood

Here's how a sample set of Markdown files would be converted.

- README.md -> index.html
- log1.md -> log1.html
- log2.md -> log2.html
- notes.md -> notes.html

Initially, all log files are placed in the `/docs` folder. This will create the html files in the root of your GitHub Pages repo site.

It is possible to create a folder structure to hold additional Markdown files. These would then be converted to HTML and hosted on GitHub Pages.

Here's the mapping.

| GitHub Repo source | GitHub Pages URL |
| --- | --- |
| `https://github.com/<username>/100-days-log/docs/` | `https://<username>.github.io/100-days-log/` |

Here are some paths and their URL mapping.

| GitHub Repo source | GitHub Pages URL |
| --- | --- |
| `/docs/README.md` | `https://<username>.github.io/100-days-log/index.html` |
| `/docs/log1.md` | `https://<username>.github.io/100-days-log/log1.html` |
| `/docs/my-notes.md` | `https://<username>.github.io/100-days-log/my-notes.html` |
| `/docs/logs/page1.md` | `https://<username>.github.io/100-days-log/logs/page1.html` |
| `/docs/school-notes/cs101.md` | `https://<username>.github.io/100-days-log/school-notes/cs101.html` |

### Reference
![100 Days of Code by James Priest](https://james-priest.github.io/100-days-of-code-log/)

### Getting Started
GitHub Pages uses [Jekyll](https://jekyllrb.com/) to build the static site. Jekyll is a Ruby-based static site generator that uses [Liquid](https://jekyllrb.com/docs/liquid/) as it's templating language and Markdown as it's content source. Code logs are written in Markdown.

In order to preview and test changes, Jekyll GitHub Pages  should be installed locally. GitHub recommends installing Jekyll to preview your site and help troubleshoot any failed Jekyll builds.

While Jekyll relies on Ruby and Liquid for logic and templating, you don't need to know anything other than Markdown in order to create your log. Here are a couple Markdown resources.

- [GitHub Guides Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
- [Markdown Syntax Cheatsheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)

### Prerequisites

[Ruby](https://www.ruby-lang.org/) and [Bundler](http://bundler.io/) need to be installed before proceeding.

1. Open the terminal (Terminal, Git Bash, WSL, etc.).
2. Check whether you have Ruby 2.1.0 or higher installed:

   ```bash
   $ruby --version
   > ruby 2.X.X
   ```

3. If you don't have Ruby installed, [install Ruby 2.1.0 or higher](https://www.ruby-lang.org/en/downloads/).
4. Install Bundler:

   ```bash
   $ gem install bundler
   # Installs the Bundler gem
   ```

### Installation

Fork and clone the repo, then use Bundler to install the gem dependencies.

1. Fork the repo by clicking the Fork button in the upper right corner of the page.

    ![Fork button](./docs/src/fixed/fork.jpg)

2. Clone (or download) the repo.

    ```bash
    $ git clone https://github.com/<username>/100-days-log.git
    $ cd 100-days-log/docs/
    >
    ```

3. Install Jekyll and other [dependencies](https://pages.github.com/versions/) from the GitHub Pages gem with the following command.

    ```bash
    $ bundle install
    > Fetching gem metadata from https://rubygems.org/............
    > Fetching version metadata from https://rubygems.org/...
    > Fetching dependency metadata from https://rubygems.org/..
    > Resolving dependencies...

### Usage

You can serve the site and enable live-reload if desired. [Additional command line options](https://jekyllrb.com/docs/configuration/options/) exist to changes things such as port, hostname, url, etc.

### Serve site

Serves the local Jekyll site and rebuilds anytime a source file changes.

1. Navigate to the `docs` folder off of the root directory.
2. Run the Jekyll site locally.

    ```bash
    bundle exec jekyll serve
    ```

3. Preview your local Jekyll site in your web browser at

     [http://localhost:4000](http://localhost:4000)

### Serve site (with with live-reload)

Serves, builds and auto-reloads the page when whenever a source file changes.

1. Navigate to the `docs` folder off of the root directory.
2. Run the Jekyll site locally.

    ```bash
    bundle exec jekyll serve --livereload
    ```

3. Preview your local Jekyll site in your web browser at

     [http://localhost:4000](http://localhost:4000)

