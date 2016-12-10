# rails-vagrant-box
Vagrant box for Ruby on Rails

## Clone the repository and vagrant init
   vagrant init -m rails

## vagrant up
    vagrant up

## Add a new project
    rails new tmpapp

## Go to project
    cd tmpapp

## Run Rails Server
    rails s -b 192.168.33.10

## View in Browser
    http://192.168.33.10:3000/

### Extras
    if Rails seems to be complaining that we’re accessing it from the host (192.168.33.1), but it renders the console just fine in our browser so that message is just noise to us.
    To get rid of it, you can follow the advise in this SO question, i.e. add this to config/environments/development.rb:
        config.web_console.whitelisted_ips = '192.168.33.1'

### Resources from
    http://justincalleja.com/2015/12/26/ruby-on-rails-vagrant-box/
