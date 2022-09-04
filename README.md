Setting up and running local server.

```bash
# https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll
# Setup docs as the source folder in Github actions. 
mkdir docs ; cd docs ; 
sudo gem install jekyll
jekyll new --skip-bundle .
bundle install
bundle update github-pages
bundle exec jekyll serve
```