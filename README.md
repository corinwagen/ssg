# ssg

### Introduction

This is a minimal static site generator written in Go. I am not proficient in Go. 
This SSG is partly an exercise to help me learn a new language, so I make no guarantees re: code quality.

### Structure

There are two types of pages supported here: "blog" pages and "regular" pages. 

``src/`` contains the pages (in HTML) with a FrontMatter heading. All this code is embedded directly in the resulting page. 

``static/`` contains files which aren't frequently changed: page templates and stylesheets.

``public/`` contains the finished pages.

  ``public/blog/`` contains the finished blog posts.

### Usage

From the index directory, run:

```
$ go run build.go
```

This creates new pages in ``public/`` by combining the raw pages in ``src/`` with the templates from ``static/``. That's all there is!

### License

This project is licensed under the Apache License, Version 2.0.

*Copyright 2021 by Corin Wagen*

