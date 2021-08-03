**Purpose:**
This goal is to assist security engineers, developers and architects to perform security testing against their web application, cloud environment, mobile app or IoT.

## Evolution
> It is quite a fuss for a developer or security tester to perform detailed penetration test against what they have built. Especially, if you do not have access to the required tools. The ultimate goal of this program is to solve this problem providing an complehensive tool set andhow to guide.

# Table of contents

1. [Overview](#overview)
2. [Methodology](#methodology)
    1. [Cloud](#cloud)
3. [Routes](#routes)

## Overview

## Methodology <a name="methodology"></a>
A general methodology can be used and tweaked for specific use cases.
- **Information gathering, version of application/server by inspecting response headers**
- **Access Handling, understand mechanism of registration/login/logout/data attacks**
- **Test Session mgmt, session cookies, flags set, CSRF**
- **Authentication tests, Info leakage, error handling**
- **Input Handling**
- **Appllication Hosting, AWS Console, test webserver** 
- **Webscraping and DNS checks for assosciated target domains**
- **Infra hardening checks (DB, Linux and network)**



### Gems files to add <a name="gems"></a>
```ruby
gem 'bourbon'
gem 'crack'
gem 'jquery-rails'
gem 'json'
gem 'meta-tags', '~> 2.1'
gem 'net-scp'
gem 'net-ssh'
gem 'pygments.rb'
gem 'redcarpet'
gem 'sidekiq'
gem 'sidekiq-failures'
gem 'sitemap_generator'
