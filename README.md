**Purpose:**
This tool is built to aid security engineers, developers and architects to identify the attack surface of a target organisation.

## Evolution
> It is quite a fuss for a developer or security tester to perform an analysis of your domain's attack surface and dangerous ports. Especially, if you do not have access to the required tools. The ultimate goal of this program is to solve this problem providing an automated tool; **running multiple scanning tools to discover vulnerabilities, effectively judge false-positives, collectively correlate results** and **saves precious time**; all these under one roof.<p>Enter **Ceziam**.

## Features
- **one-step security check**.
- **dangerous port check** 
- **attack surface check by enumaerating subdomains**  
- **displays the results spontaneously**
- **Future versions will include API security verification and WebApplication OWASP top10 checks**
- saves a lot of time, **indeed a lot time!**

## Bug Reports
> Ceziam uses Github Issues to keep track of bug reports. Please be sure to include the component of Ceziam that had the issue, steps to reproduce the bug, and a description of what you expect to be the correct behavior.

## Pull Requests
> Ceziam welcomes your code contribution in the form of a Github Pull Request. We will review your request (normally nor more than a day or so)and then merge. We will be sure to properly credit you in the CHANGELOG file, and the commit message will reference the PR number.

Please feel free to connect to ceziam.com and use this feely available Cyber Security tool.

# Ceziam, How It Was Written 
# Table of contents

1. [Overview](#overview)
    1. [Skeleton](#skeleton)
    2. [Gem files to add](#gems)
2. [Frontend](#frontend)
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
### Skeleton <a name="skeleton"></a>
```bash
rails new \
--database postgresql \
--webpack \
-m https://raw.githubusercontent.com/lewagon/rails-templates/master/devise.rb \
ceziam
```
- Versions: `Rails 6.0.3.1` `ruby 2.6.6p146`
- Install Node locally from here https://nodejs.org/en/download/
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
