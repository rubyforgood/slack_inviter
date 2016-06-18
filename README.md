# Ruby for Good Slack Invatation

The source for [Ruby for Good's Slack Inviter](https://rubyforgood.herokuapp.com/).

The application based [Andy Lindeman's](https://github.com/alindeman) [ATLDevs automatic invitation system](https://github.com/alindeman/atldevs).


## Prerequisites

* PostgreSQL: `brew install postgresql`
* Redis: `brew install redis`

## Required Configuration

Configuration items are stored in environment variables.

* `SLACK_SUBDOMAIN`: e.g., rubyforgood for rubyforgood.slack.com
* `SLACK_TOKEN`: an API token for an administrator of the organization
* `SIDEKIQ_USERNAME`: username for the sidekiq administration area
* `SIDEKIQ_PASSWORD`: password for the sidekiq administration area

## Deployment

Deployed on Heroku. Ask info@rubyforgood.org for access. In production, we run a puma process in the same dyno as a sidekiq worker. It's a hack to keep it free.
