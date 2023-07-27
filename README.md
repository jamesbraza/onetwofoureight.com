# onetwofoureight.com

Files underpinning https://onetwofoureight.com/

## Website

The website is hosted via [GitHub Pages](https://pages.github.com/).
It was made with the static site generator [Hugo](https://gohugo.io/),
and the theme is [Hermit](https://themes.gohugo.io/themes/hermit/)
([repo](https://github.com/Track3/hermit)).

## Developers

### `.gitignore`

Here's how I constructed the `.gitignore`:

```bash
curl -s \
  https://raw.githubusercontent.com/github/gitignore/master/{Global/Vim,Global/VisualStudioCode,Global/macOS,community/Golang/Hugo}.gitignore \
  > .gitignore
```

## Style

Markdown content in this website are written using [semantic linefeeds][1].

[1]: https://rhodesmill.org/brandon/2012/one-sentence-per-line/
