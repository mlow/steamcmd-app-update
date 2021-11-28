# steamcmd-app-update

Outputs one `app_update <app-id> [-validate]` line per game in your Steam
library.

A useful tool if you intend to automate the fetching of your entire library :)

# Configuration

Configuration is done via environment variables as opposed to CLI flags:

```sh
# Steam API key.
export STEAM_API_KEY=

# The profile ID to fetch the list of owned games of.
export STEAM_PROFILE_ID=

# Comma separated list of game names or App IDs to skip
export SKIP_GAMES='Dota 2 Test, Metro Exodus, 1240440'

# Whether to force game file validation by adding -validate
# Any value = true, unset/empty = false
export FORCE_VALIDATE=

# Output file (optional, defaults to stdout)
export OUTPUT_FILE=
```

# Limitations

* Cannot conveniently filter game output by platform (Windows, Mac, Linux)
