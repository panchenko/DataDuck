# Getting Started

## Requirements

DataDuck ETL currently supports extracting from MySQL and PostgreSQL databases. It supports loading into Amazon
Redshift. If you would like to extract or load into a database not yet supported, contact us.

## Instructions

First, create a new, empty directory. Inside this directory, create a file named Gemfile with the following:

```ruby
source 'https://rubygems.org'

gem 'dataduck'
```

Then execute:

    $ bundle install

Finally, run the quickstart command:

    $ dataduck quickstart

It will ask you for the credentials to your database, and then create the basic setup for your project. After the setup, your project's ETL can be run by running `ruby src/main.rb`

If you would like to run this regularly, such as every night, it's recommended to use the [whenever](https://github.com/javan/whenever) gem to manage a cron job to regularly run the ETL.