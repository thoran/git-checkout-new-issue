# git-checkout-new-issue

## Description

Simultaneously create a new issue and a new branch to match.

## Installation

### 0. Have a recent version of Ruby installed

### 1a. Via Homebrew

```shell
$ brew tap thoran/tap
$ brew install thoran/tap/git-checkout-new-issue
```

### 1b. Manually

```shell
$ git clone https://github.com/thoran/git-checkout-new-issue
$ cp ./git-checkout-new-issue/bin/git-checkout-new-issue to your preferred executable path
$ chmod +x /path/to/git-checkout-new-issue
```

## Usage

### 1. If `git` is installed
```shell
$ git checkout-new-issue
```

### 2. If `git` is not installed (though I'm not sure why you'd want this installed if it wasn't)
```shell
$ git-checkout-new-issue
```

### 3. It is expected that this will be aliased to something a bit shorter
```shell
$ cat ~/.config/git/config
...
[alias]
  coni = checkout-new-issue
...
$ git coni
```

## Notes

1. `.env.development.local` is expected to be left out of the repo, so that each dev is able to create their own keys.
2. This is Jira only for now.

## Contributing

1. Fork it: `https://github.com/thoran/git-checkout-new-issue/fork`
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Create a new pull request
