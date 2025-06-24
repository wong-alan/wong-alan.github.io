# Alan's Annals
Musings and snippets from my thoughts.

#### Running locally
`bundle exec jekyll serve`
___
### Jekyll Installation
[Jekyll Docs](https://jekyllrb.com/docs/installation/windows/)
#### Process for WSL on Windows 11
Instead of installing Ruby from BrightBox, just follow the [Ruby docs](https://www.ruby-lang.org/en/documentation/installation/#apt) \
When installing Jekyll, if you run into `You don't have permissions for the <gems> directory`, run with `--user-install`
 * `gem install jekyll bundler --user-install`

If you run into the warning `You don't have <Ruby bin> in your PATH, gem executables will not run`, add it to your `$PATH`
 * For `.zsh`:
 ```
 path+=('<Ruby bin>')
 export PATH
 ```
 then run `exec zsh`

If you run into `Bundler::PermissionError There was an error while trying to write to <gem dir>` while running `bundle`, add a new `GEM_HOME` to your environment.
 * In `.zsh`:
 ```
export GEM_HOME=$HOME/.gem
 ```
 then run `exec zsh`