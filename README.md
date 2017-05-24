# dokku-git-revision

Captures the git revision and makes it available at /app/REVISION.

The revision is stored inside the image so that the correct revision is available despite a rollback or any kind of deployment issue.


## Requirements

* dokku 0.4.4+ (tested on 0.9.4)


## Installation

```
dokku plugin:install https://github.com/zarqman/dokku-git-revision.git
```


## Hooks

This plugin provides one hook:

* `pre-receive-app`: captures and stores the git revision


## Usage

Works automatically on all git deploys.


## License

MIT
