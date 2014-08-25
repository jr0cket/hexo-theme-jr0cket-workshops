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

