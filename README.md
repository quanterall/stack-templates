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

`template-name` here is a stand-in for the available templates in this directory,
which (currently) means you can replace it with `basic`, `application` or
`web-postgres`.