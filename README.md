# Women in Machine Learning static page generator

## Getting started with Hugo

* [Installation](https://gohugo.io/installation/)
* For Mac, I would recommend installing [Homebrew](https://brew.sh/) and install 
Hugo via the terminal (`brew install hugo`)

## Download a template (optional)

* Themes can be found here: [Hugo Themes](https://themes.gohugo.io/)
* We use Roxy Hugo: 
[[Hugo Template](https://themes.gohugo.io/themes/roxo-hugo/)] 
[[Github Repo](https://github.com/StaticMania/roxo-hugo)]

## Create a Hugo project with template (optional, already done here)

Terminal (bash):

```
# create Hugo project
hugo new site webpage
cd webpage

# Add the repository into your Hugo Project repository as a submodule
git submodule add git@github.com:StaticMania/roxo-hugo.git themes/roxo-hugo

#Copy the data, content, static, resources & config.toml files from the 
# exampleSite directory and paste it on you Hugo Project repository/directory. 
cp -a themes/roxo-hugo/exampleSite/* .
```

## Preview the webpage locally

Terminal (bash):

```
hugo server -F

# Exemplary output on the terminal:
#
# Start building sites …
# hugo v0.110.0+extended darwin/arm64 BuildDate=unknown
# 
#                    | EN
# -------------------+-----
#   Pages            | 24
#   Paginator pages  |  2
#   Non-page files   |  0
#   Static files     | 52
#   Processed images |  0
#   Aliases          |  2
#   Sitemaps         |  1
#   Cleaned          |  0
# 
# Built in 56 ms
# Watching for changes in /Users/linhtran/Documents/workspace/webpages/womeninml/webpage/{archetypes,assets,content,data,layouts,static,themes}
# Watching for config changes in /Users/linhtran/Documents/workspace/webpages/womeninml/webpage/config.toml
# Environment: "development"
# Serving pages from memory
# Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
# Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
# Press Ctrl+C to stop
```

Webpage can be viewed at [localhost:1313](http://localhost:1313/)

## Publish the site 

When you publish your site, Hugo creates the entire static site in the public directory in the root of your project. This includes the HTML files, and assets such as images, CSS files, and JavaScript files.

```
hugo
```