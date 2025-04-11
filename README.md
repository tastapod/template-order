# Sample Hugo website to demonstrate behaviour change in new template system

This mini-site is to support [gohugoio/hugo#13588](https://github.com/gohugoio/hugo/issues/13588).

The new template system introduced in Hugo 0.146 has a different lookup algorithm to 0.145 and earlier. In particular, it seems to ignore `layout = {'single'|'list'}` values in section index pages, routing them all to `section.html`.

This may just be breaking for these specific values, but it is a breaking change in default behaviour that I rely on for <dannorth.net> among other sites.
