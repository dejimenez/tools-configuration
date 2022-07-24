# asdf

`asdf` is a tool version manager. All tool version definitions are contained within one file (.tool-versions) which you can check in to your project's Git repository to share with your team, ensuring everyone is using the exact same versions of tools.

[Website](https://asdf-vm.com/)

## Install asdf on Mac

1. brew install asdf
2. echo -e "\n. $(brew --prefix asdf)/libexec/asdf.sh" >> ${ZDOTDIR:-~}/.zprofile
3. run `asdf` to list all possible commands

> Note: in older versions of Mac the file could be `.zshrc` instead of `.zprofile`

## Install plugin

1. asdf plugin list all
2. `asdf plugin list all | grep python` to filter by specific plugin 
3. asdf plugin add python
4. asdf plugin list

> Note: Some plugin could requires dependencies.

## Intasll version

1. asdf list all python
2. asdf install python 3.10.5
3. asdf global python 3.10.5

> Some versions like `java` plugin require further configuration, check the github documentation to

## Install system existing tool Ex: `ruby`
```
https://mac.install.guide/ruby/6.html
```

It is similar to install another kind of plugin + tool

1. asdf plugin add ruby
2. asdf list all ruby
3. asdf install ruby latest
4. asdf global ruby 3.1.2

> Note: in this case the installed version was the `latest`, in some cases is possible to also install `lts` version. It is also possible to install specific version.