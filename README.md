# Ze-ultimate-setup

Notes and resources for configuring my Windows &amp; Mac computers

## Windows

### Git & Bash

Install Git for Windows:

https://gitforwindows.org/


Set gitconfig to (change to your name / public github email)

```
[user]
        email = 1448524+mxro@users.noreply.github.com
        name = Max Rohde

[core]
        autocrlf = false
```

Use Git Bash terminal for VSCode:

```
  "terminal.integrated.profiles.windows":{"Git Bash":{"path":"C:\\Program Files\\Git\\bin\\bash.exe"},  },
  "terminal.integrated.defaultProfile.windows": "Git Bash",
```

Set up SSH key: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

Ensure to:

```
# start ssh agent
eval $(ssh-agent -s)

# add your key
ssh-add ./.ssh/id_ed25519

# check key is added
ssh-add -l

# scan for new keys
ssh-keyscan github.com >> ~/.ssh/known_hosts
```


### PowerToys

#### Installation

[Install](https://learn.microsoft.com/en-us/windows/powertoys/install)

#### Configuration

- Disable all modules but 'PowerToys Run'