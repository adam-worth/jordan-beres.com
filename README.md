# jordan-beres.com

The code for my [website](https://www.jordan-beres.com) built with jekyll.
Cloned and recreated with my information based off of [chicochico's](https://github.com/chicochico/fchiang.com) project.

## Running locally
Build:
```
docker build -t jekyll .
```

Run:
```
docker run --rm -p 4000:4000 --entrypoint bash jekyll -c \
'bundler exec jekyll serve -H 0.0.0.0 -P 4000'
```

For development with live reload:
```
docker run -it --rm -v $(pwd):/app -p 4000:4000 -p 35729:35729 --entrypoint bash jekyll -c \
'bundler exec jekyll serve -H 0.0.0.0 -P 4000 --livereload'
```

See the preview [here](localhost:4000).
