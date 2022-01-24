# CLI

## Shell

I use `zsh`. I don't have strong opinions on shells and correspondingly my shell is bells and whistle free. This is my whole `.zshrc`

```bash
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"

export PATH="$HOME/.poetry/bin:$PATH"
export PYTHONPATH=$PWD

export PATH="/Users/nsayre/Desktop:$PATH"
```

Added `/Users/nsayre/Desktop` because I like to do bad things.

## Fun Commands

1. `which`

    I find myself on the terminal way too often trying to figure out which (pun unintended) version of a program is running. Usually this program is Python

    ```bash
    which python
    ```
