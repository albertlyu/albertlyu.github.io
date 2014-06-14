albertlyu.github.io
===================

## Overview
A repository for my website at http://www.albertlyu.com/.

## Resume in Markdown
Forked from [David Hamp-Gonzalves' repo](https://github.com/davidhampgonsalves/resume):

This my resume in markdown format which lets me version, style and generate html and pdf formats using https://github.com/c0bra/markdown-resume-js. The current style supports printing and mobile devices.

###setup
* first: npm install (which installs [markdown-resume](https://github.com/there4/markdown-resume))
* second: remove the existing core css files in `node_modules/markdown-resume/assets/css` and move `resume.css` into that dir.
* third: move `default.html` into `node_modules/markdown-resume/assets/templates` to add Google Analtyics.


__to generate PDF's you'll also need to install: [wkhtmltopdf](https://github.com/pdfkit/pdfkit/wiki/Installing-WKHTMLTOPDF)__.

###generate
```shell
node node_modules/markdown-resume/bin/md2resume resume.md
node node_modules/markdown-resume/bin/md2resume --pdf resume.md
```