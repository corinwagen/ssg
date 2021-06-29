# ssg

### Introduction

This is a minimal static site generator written in Go. I am not proficient in Go. 
This SSG is partly an exercise to help me learn a new language, so I make no guarantees re: code quality.

### Structure

There are two types of pages supported here: "blog" pages and "regular" pages. 

``src/`` contains the pages (in HTML) with a FrontMatter heading. All this code is embedded directly in the resulting page. 

``static/`` contains files which aren't frequently changed: page templates and stylesheets.

``public/`` contains the finished pages.

### Usage

To adapt this project for your own use, simply update the templates in ``static/`` as desired, and add new content to ``src/.``
Then, from the index directory, run:

```
$ go run build.go
```

This creates new pages in ``public/`` by combining the raw pages in ``src/`` with the templates from ``static/``. That's all there is!

### License

This project is licensed under the Apache License, Version 2.0.

*Copyright 2021 by Corin Wagen*

