# iBot Robotics Club, IIT Madras

This is the repository for iBot Club, Indian Institute Of Technology, Madras.

Hosted at: [iBot Official Site](https://a-jacked-nerd.github.io/ibot_iitm_website/)

### Development

First off, you'll need to **[install Ruby](https://www.digitalocean.com/community/tutorials/how-to-install-ruby-on-rails-with-rbenv-on-ubuntu-16-04)**. You should not be installing Jekyll directly, since that's likely to break things. Instead, install bundle with

```gem install bundle```

Avoid spaces between any of the directory names. Use underscore insted.

Then, execute these in the repo directory:

```
bundle install --path vendor/bundle
bundler exec jekyll server --port 8080 --host 0.0.0.0
```
Here the --path flag is optional to keep your system's packages sane.

Before committing execute this in the repo directory:
```
bundle exec jekyll build
```
