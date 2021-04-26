# Quanterall templates for Haskell development

This is a collection of templates for development of Haskell applications. They
all feature development containers meant to be used with VSCode. That feature in
itself requires `docker` and `docker-compose`, but once a project is set up you
only need those two tools as well as VSCode to participate in development.

Note that usage of the templates requires the tool `stack`, so if you're looking
to generate new projects it's useful to
[install stack](https://docs.haskellstack.org/en/stable/install_and_upgrade/).

## Using the templates

Once you have `stack` you can use our templates as follows:

```bash
stack new my-project-name quanterall/template-name
```

## Available templates

### `basic`

Basic template with minimal structure for making executables, good for small
projects/experiments. This purposefully has no libraries included by default,
which is likely appropriate for when you don't want to presume the need for
anything in particular, or want a light template for a library, where you will
add the smallest set of dependencies you need.

### `application`

[RIO](https://www.stackage.org/package/rio)-based application with command line
parsing & logging added by default, likely a good choice for most non-web
applications.

The application layout is, again, based on
[RIO](https://www.stackage.org/package/rio) which should likely make it the
default choice for an application that needs/ought to keep mutable state over a
longer execution time, as well as take advantage of `RIO` as a `Prelude`
alternative.

### `web-postgres`

Web-template using the framework Yesod:

Includes models, controllers, routing, templates, etc. by default. Uses postgres,
as the name implies.

`Yesod`, with associated learning material, can be found
[here](https://www.yesodweb.com/).
