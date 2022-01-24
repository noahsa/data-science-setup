# Visual Studio Code

## Features

1. Python debugger - I use the debugger ALL the time
2. Git Integration - Especially useful for git diffs. Wish it worked better with pre-commit. I run all git commands on the terminal, except when I'm lazy

### Debugger Setup

There are several ways to setup the debugger, it all ends with a `.vscode/launch.json`. The below is my typical file. Two things to note:

1. The python configuration points at the Python in my project's virtual environment
2. I am passing in arguments. Many of my applications are parameterized with CLI arguments.

```json
{
"version": "0.2.0",
"configurations": [
        {
            "name": "Python: Current File",
            "type": "python",
            "request": "launch",
            "program": "${file}",
            "justMyCode": false,
            "console": "integratedTerminal",
            "python": "./venv/bin/python",
            "args": ["--argument1", "1"
                     "--argument2", "2"
                    ]
        }
    ]
}
```
