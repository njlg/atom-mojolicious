# Atom Mojolicious

[Mojolicious](http://mojolicio.us) support for [Atom.io](http://atom.io). This is very similar to the [Sublime Text Mojolicoius](https://github.com/SublimeText/Mojolicious) plugin.

## Description

This plugin has a syntax, completions, and snippets for working with Mojolicious Embedded Perl templates.

## Completions

Inside a Embedded Perl block the following completions are available:

`app`
`content`
`content_for`
`dumper`
`extends`
`include`
`flash`
`layout`
`layout`
`memorize`
`param`
`session`
`stash`
`url_for`
`title`
`base_tag`
`check_box`
`file_field`
`form_for`
`hidden_field`
`input_tag`
`javascript`
`link_to`
`password_field`
`radio_button`
`select_field`
`stylesheet`
`submit_button`
`tag`
`text_area`
`text_field`

## Snippets

### EP Templates

From an EP template you can use these snippets:

`app` &rarr; `app->`

`content_for` &rarr; `content_for ${name} => begin`

**Note**: I have the following defined, but they don&rsquo;t seem to work.

`<%` &rarr; `<% $1 %>`

`<%=` &rarr; `<%= $1 %>`

`<%==` &rarr; `<%== $1 %>`

### Perl

From a Mojolicious controller (or any perl source) you can use these snippets:

`debug` &rarr; `$self->app->log->debug(${1:'debug message'});`

`error` &rarr; `$self->app->log->error(${1:'error message'});`

`mdump` &rarr; `$self->app->log->debug($self->dumper(${1:object}));`
