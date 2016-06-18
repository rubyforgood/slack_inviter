# Ruby for Good Slack Invatation

The application based on the application behind the [ATLDevs automatic invitation system](https://atldevs.herokuapp.com)

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
