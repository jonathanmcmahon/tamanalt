# TAMANALT

Tamanalt is a responsive theme for [Pelican](http://getpelican.com) based on [Karambir Nain's taman theme])https://github.com/karambir/taman).

## DEMO

You can see the theme in use [here](http://jmcmahon.org).

## INSTALL

Clone the repository, edit `pelicanconf.py` and modify the `THEME` variable to make it point to the downloaded theme location.

The theme uses the *assets* plugin to handle minification of css files from [here](https://github.com/getpelican/pelican-plugins/tree/maser/assets)

- Install required package for *assets* plugin by `pip install webassets`
- Refer this [documention](https://github.com/getpelican/pelican-plugins#how-to-use-plugins) to install plugin.

## PELICANCONF.PY

Supports a number of common global variables but patches are welcomed if you need better support.

- `GOOGLE_ANALYTICS` to use Google Analytics, set this var to your UA-XYZ code

- `DISQUS_SITENAME` set this to your Disqus sitename to enable disqus comments in articles

- `TAGLINE` some text rendered right below the logo

- Use `canonical_url` var in article markdown file to specify original url of article.

- To set custom logo and favicon set following in config:

    STATIC_PATHS = ['images', 'extra/favicon.png', 'extra/logo.png']
    EXTRA_PATH_METADATA = {
        'extra/favicon.png': {'path': 'favicon.png'},
        'extra/logo.png': {'path': 'logo.png'},
    }

    USER_LOGO_URL = '/logo.png'
    USER_FAVICON_URL = '/favicon.png'

When developing locally, you may want to set the following variable: `SITEURL = http://localhost:8000`

## AUTHOR

Taman was originally authored by [Karambir Nain](https://github.com/karambir). I started with his theme [taman](https://github.com/karambir/taman) and customized it for my purposes.
