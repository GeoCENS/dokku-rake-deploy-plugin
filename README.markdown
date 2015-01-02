# Dokku Rake Deploy Plugin

Will trigger custom rake tasks after an app is deployed using Dokku.

## Installation

To install, checkout the repository to your Dokku plugins directory and update the Dokku plugins:

    # cd /var/lib/dokku/plugins
    # git clone <repo url>
    # dokku plugins-install

The plugin is then installed. You can see it is installed if it appears in the dokku help list:

    # dokku help
    …
        rake-deploy <app>
        rake-deploy:set <app> <task> [task...]
        rake-deploy:clear <app>
    …

## Usage

Once installed you can set the rake task using the set command:

    # dokku rake-deploy:set <app> deploy:check deploy:notify

The other commands should be self-explanatory.

## License

MIT License
