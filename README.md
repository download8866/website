# Website

Nothing to see here, just the static files that serve micro.mu

## Usage

- Generate the docs
- Generate the blog
- Generate the CN blog

```
# docs
cd github.com/micro/docs
jekyll build
rsync -avz --delete _site/ ../website/html/docs/

# blog
cd github.com/micro/blog
jekyll build
rsync -avz --delete _site/ ../website/html/blog/

# CN blog
cd github.com/micro-in-cn/blog
jekyll build
rsync -avz --delete _site ../../micro/website/html/blog/cn/
```
