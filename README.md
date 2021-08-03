**Purpose:**
This goal is to assist security engineers, developers and architects to perform security testing against their web application, cloud environment, mobile app or IoT.

## Evolution
> It is quite a fuss for a developer or security tester to perform detailed penetration test against what they have built. Especially, if you do not have access to the required tools. The ultimate goal of this program is to solve this problem providing an complehensive tool set andhow to guide.

# Table of contents

1. [Overview](#overview)
2. [Methodology](#methodology)
    1. [Views](#views)
3. [Routes](#routes)
4. [Controller](#controller)
5. [Models](#model)
    1. [checks table](#checks)
6. [Attack Engine](#attackengine)
    1. [Attack Calls](#attackcalls)
7. [Java Scripts Used](#js)
    1. [Timer check for script to run](#timerjs)
8. [Redis and Heroku](#redisandheroku)
    1. [Useful Heroku comamnds](#herokucommands)
    2. [Sidekiq overview and how to deploy to Heroku](#sidekiq)
    23. [Sidekiq overview and how to deploy to Heroku](#sidekiq)

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
