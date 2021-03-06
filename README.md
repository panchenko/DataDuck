# DataDuck ETL

##### Set up in under 5 minutes

DataDuck ETL is probably the quickest extract-transform-load framework system to set up. If you want to set up a data warehouse, give DataDuck ETL a try.

##### Extract-transform-load to Amazon Redshift

DataDuck ETL is currently focused on loading to Amazon Redshift (through Amazon S3).

![DataDuck ETL](static/logo.png "DataDuck ETL")

## Installation

##### Instructions for using DataDuck ETL

Create a new, empty directory. Inside this directory, create a file named Gemfile, and add the following to it:

```ruby
source 'https://rubygems.org'

gem 'dataduck'
```

Then execute:

    $ bundle install

Finally, run the quickstart command:

    $ dataduck quickstart

The quickstart wizard will ask you for credentials to your database, then create the basic setup for your project. After the quickstart, you'll still need to edit the .env and config/base.yml files, as well as customize your tables. Finally, your project's ETL can be run by running the `dataduck etl all` command.

If you'd like to run this regularly, such as every night, it's recommended to use the [whenever](https://github.com/javan/whenever) gem to manage a cron job to regularly run the ETL.

## Documentation

Visit the [docs page](http://dataducketl.com/docs/overview/welcome) to read the documentation. The docs page is autogenerated from the files in this project's docs directory.

## Contributing

To contribute, get in touch at http://DataDuckETL.com/ so that we can share the [Contributor License Agreement (CLA)](https://en.wikipedia.org/wiki/Contributor_License_Agreement) with you, then create a pull request.

## License

Get in touch or visit [http://dataducketl.com/licensing](http://dataducketl.com/licensing) for licensing.
