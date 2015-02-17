## Sensu-Plugins-messagemedia

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-messagemedia.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-messagemedia)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-messagemedia.svg)](http://badge.fury.io/rb/sensu-plugins-messagemedia)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-messagemedia/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-messagemedia)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-messagemedia/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-messagemedia)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-messagemedia.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-messagemedia)

## Functionality

## Files
 * bin/handler-messagemedia

## Usage

```
{
  "messagemedia": {
    "username": "username",
    "password": "password",
    "mobile_numbers": ["+123456789", "+987654321"]
  }
}
```

## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-messagemedia -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-messagemedia`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-messagemedia' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-messagemedia' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
