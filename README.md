# Website

## WSL2

### Set up

On a home directory,

```
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'eval "$(~/.rbenv/bin/rbenv init - bash)"' >> ~/.bashrc
git clone https://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build
sudo apt install -y build-essential libssl-dev libreadline-dev zlib1g-dev \
                    libyaml-dev libffi-dev autoconf bison \
                    libgdbm-dev libncurses5-dev pkg-config libssl-dev
rbenv install 3.4.7
rbenv global 3.4.7
rbenv exec gem install bundler
gem update --system 3.7.2
gem install middleman
```

### Build

On Website Directory

```
middleman build
```

