---
date: 2019-01-20T17:08:38Z
title: "jx create git token"
slug: jx_create_git_token
url: /commands/jx_create_git_token/
---
## jx create git token

Adds a new API token for a user on a Git server

### Synopsis

Creates a new API Token for a user on a Git Server

```
jx create git token [username] [flags]
```

### Examples

```
  # Add a new API Token for a user for the local Git server
  # prompting the user to find and enter the API Token
  jx create git token -n local someUserName
  
  # Add a new API Token for a user for the local Git server
  # using browser automation to login to the Git server
  # with the username and password to find the API Token
  jx create git token -n local -p somePassword someUserName
```

### Options

```
  -t, --api-token string          The API Token for the user
  -b, --batch-mode                In batch mode the command never prompts for user input
      --headless                  Enable headless operation if using browser automation
  -h, --help                      help for token
      --install-dependencies      Should any required dependencies be installed automatically
      --log-level string          Logging level. Possible values - panic, fatal, error, warning, info, debug. (default "info")
  -n, --name string               The name of the Git server to add a user
      --no-brew                   Disables the use of brew on macOS to install or upgrade command line dependencies
  -p, --password string           The User password to try automatically create a new API Token
      --pull-secrets string       The pull secrets the service account created should have (useful when deploying to your own private registry): provide multiple pull secrets by providing them in a singular block of quotes e.g. --pull-secrets "foo, bar, baz"
      --skip-auth-secrets-merge   Skips merging a local git auth yaml file with any pipeline secrets that are found
      --timeout string            The timeout if using browser automation to generate the API token (by passing username and password)
  -u, --url string                The URL of the Git server to add a user
      --verbose                   Enable verbose logging
```

### SEE ALSO

* [jx create git](/commands/jx_create_git/)	 - Creates a Git resource

###### Auto generated by spf13/cobra on 20-Jan-2019
