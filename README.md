# Overview 

A theme designed to make it easier to create workshops for developers.


# Install

Create a new project with Hexo.io

    hexo init project-name
    cd project-name
    npm install 
    git clone https://github.com/jr0cket/hexo-theme-jr0cket-workshops.git themes/workshops

Edit the Hexo project configuration file, `_config.yml` and change the theme setting to workshops

    theme: workshop


# Trying out the theme

Run the Hexo server and browse to http://localhost:4000/ to see the generated website


# Customising the theme 

## Changing the front page 

Edit the file `index.jade` to change the content of the front page

Edit the file `layout/index.ejs` to change the structure of the page.  For example, I removed everything except the line `<%- page.content %>`.

## Workshops 

Edit the file `workshops/_config.yml` to define your own workshop navigation menu, which appears on the left hand side of the page 



## Minimising the title 
The page title is wrapped in a page-banner which is very large and takes up too much space 

Original banner for page title 

``` source/css/_partial/page.styl 
#page-banner
  @extend $banner-background
  padding: 30px 0
  text-align: center
  @media mq-normal
    padding: 40px 0
    text-align: left
```

Modification where I reduced the size of the padding

``` source/css/_partial/page.styl 
#page-banner
  @extend $banner-background
  padding: 10px 0
  text-align: center
  @media mq-normal
    padding: 10px 0
    text-align: left
```

I also removed the "edit in github" link in the title banner by removing a line from the layout file `layouts/_partial/page.ejs`

```
<a href="https://github.com/jr0cket/hexo-theme-jr0cket-workshops/blob/master/source/<%- page.path.replace(/\.html$/, '.md') %>" title="Improve this doc" id="page-edit-link"></a>
```
