# README

This is a simple reproduction of vite_ruby [issue #395](https://github.com/ElMassimo/vite_ruby/issues/395).

If you boot the app using only `rails server`, the root page will show "Screen content" (rendered by
`app/views/application/index.html.erb`).

If, however, you boot the dev server as well, `bin/vite dev`, the root page will show "Print
content" because the print styles are added to the page without a media attribute, causing them to
override the screen styles
