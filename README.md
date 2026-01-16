# Build locally

This worked for setting up a new environment as of 2025-01-16.

```bash
sudo apt install rbenv

# install dependencies for ruby-build
sudo apt install build-essential autoconf libssl-dev libyaml-dev zlib1g-dev libffi-dev libgmp-dev rustc

# install ruby-build
git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build

rbenv install --list # pick one
rbenv install 3.4.8
rbenv global 3.4.8
rbenv exec gem install system
rbenv exec gem install bundler
rbenv exec bundle install
rbenv exec bundle exec jekyll serve
```

