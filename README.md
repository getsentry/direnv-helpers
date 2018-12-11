# direnv helpers

## Installation

```
# download the script
curl -o- https://raw.githubusercontent.com/getsentry/direnv-helpers/helpers.sh >> ~/helpers.sh

# source it in your .direnvrc
echo -n "source ~/helpers.sh" >> ~/.direnvrc
```

## How to use the helpers in your projects (NVM example)

You don't even need NVM installed yet, this script will detect if it exists and prompt for installation in your project directory if it isn't.

Make sure `direnv.net` is installed and working in your shell (For MacOS just install via homebrew) `brew install direnv` and follow the prompts to have it auto load in your shell

First: If you don't already have one, create a `.nvmrc` file and specify your node version

```
echo "8.8.1" >> .nvmrc
```

Next: Create a `.envrc` file

```
echo "requires_nvm" >> .envrc
```

Direnv should prompt you to allow the script to run and voila!

## Helpers to use in your `.envrc`

```
requires_nvm
```

# Credits

- nvm utilities: https://github.com/steve-ross/direnv-helpers
