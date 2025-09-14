# onetwofoureight.com

![Lint and Test](https://github.com/jamesbraza/onetwofoureight/actions/workflows/lint-test.yaml/badge.svg)
![Deploy Site](https://github.com/jamesbraza/onetwofoureight/actions/workflows/hugo.yaml/badge.svg)

Files underpinning <https://onetwofoureight.com/>

## Website

The website is hosted via [GitHub Pages](https://pages.github.com/).
It was made with the static site generator [Hugo](https://gohugo.io/),
and the theme is a fork of [Hermit](https://themes.gohugo.io/themes/hermit/)
([base repo][2], [fork repo][3]).

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
[2]: https://github.com/Track3/hermit
[3]: https://github.com/jamesbraza/hermit
