# Flintstone

## Maturity

This software is currently in it's zygote stage.  Don't use it prematurely.

v0.0.0.1



## Overview

Flintstone is a more opinionated customization of Bedrock.

Bedrock is a modern WordPress stack that helps you get started with the best development tools and project structure.

Much of the philosophy behind Bedrock is inspired by the [Twelve-Factor App](http://12factor.net/) methodology including the [WordPress specific version](https://roots.io/twelve-factor-wordpress/).

## Features

- Everything in Bedrock 
- Unit Testing pre-configured
- Default Template based on Timber, Twig, and `laravel-mix`
- A more opinionated PHPCS setup

## Requirements

- PHP >= 7.1
- Composer - [Install](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx)

## Installation

1. Create a new project:
   ```sh
   $ composer create-project phredeye/flintstone
   ```
2. Update environment variables in the `.env` file. Wrap values that may contain non-alphanumeric characters with quotes, or they may be incorrectly parsed.

- Database variables
  - `DB_NAME` - Database name
  - `DB_USER` - Database user
  - `DB_PASSWORD` - Database password
  - `DB_HOST` - Database host
  - Optionally, you can define `DATABASE_URL` for using a DSN instead of using the variables above (e.g. `mysql://user:password@127.0.0.1:3306/db_name`)
- `WP_ENV` - Set to environment (`development`, `staging`, `production`)
- `WP_HOME` - Full URL to WordPress home (https://example.com)
- `WP_SITEURL` - Full URL to WordPress including subdirectory (https://example.com/wp)
- `AUTH_KEY`, `SECURE_AUTH_KEY`, `LOGGED_IN_KEY`, `NONCE_KEY`, `AUTH_SALT`, `SECURE_AUTH_SALT`, `LOGGED_IN_SALT`, `NONCE_SALT`
  - Generate with [wp-cli-dotenv-command](https://github.com/aaemnnosttv/wp-cli-dotenv-command)
  - Generate with [our WordPress salts generator](https://roots.io/salts.html)

3. Add theme(s) in `web/app/themes/` as you would for a normal WordPress site
4. Set the document root on your webserver to Bedrock's `web` folder: `/path/to/site/web/`
5. Access WordPress admin at `https://example.com/wp/wp-admin/`

## Bedrock Documentation

Bedrock documentation is available at [https://roots.io/docs/bedrock/master/installation/](https://roots.io/docs/bedrock/master/installation/).

<hr style="margin-bottom: 500px">

<pre>
&quot;Yes that <em>is</em> the name...
  I don't f*** know!
  	The other thing was called "Bedrock", man!?&quot;

	<small>-- A conversation that sort of *might* have happened.</small>

</pre>
