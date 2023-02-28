# My Current Code Log for #100 days of Code.
[My Current Progress](https://nerajno.github.io/100DaysOfCodeLog/index.html)

This repo is being used to track my progress for  100 Days of Code Challenge ([https://100daysofcode.com](https://100daysofcode.com)) following Alexander Kallaway's examples.This repo also uses the format of James Priest's ([repo](https://github.com/james-priest/100-days-log)) to format this log, follow the instructions on his ReadMe if you want to use this format. 

#### Todo {Current Round =>  June 7,2022 }
- [ ] Update Readme to standardize version. 
- [ ] Implement personal branding and improve story telling for whole log.
- [x] Brain storm this version.
  

## Current Mental Status
[![Groot looking ](https://media.giphy.com/media/B9XXtlIKF8wec/giphy.gif)](https://media.giphy.com/media/B9XXtlIKF8wec/giphy.gif)

### Informative Section 

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
- Link color

These items can be customized for the site.

- Favicon - replace icon in `docs/assets/images/icons/favicon.ico`
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

Initially all log files are placed in the `/docs` folder. This will create the html files in the root of your GitHub Pages repo site.

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

