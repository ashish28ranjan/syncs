# Syncs - Keep your repo up to date

Just two simple steps -

- Pull changes from remote to local
- Push changes from local to remote

## Requirements

- bash 4.0+
- jq 1.4+
- sftp

## Install

- #### syncs
    - Download https://raw.githubusercontent.com/ashish28ranjan/syncs/master/syncs
    - Put it in $PATH
    - chmod u+x /path/to/syncs
- #### jq
    - Download jq binary from https://stedolan.github.io/jq/download
    - Put it in $PATH
    - Rename it to jq
    - chmod u+x /path/to/jq

## Commands
  - **-c | cleanup** : Delete the temporary directories
  - **-cc | config** : Create a config file in the current directory
  - **-h | help** : Display help
  - **-i | install** : Display install instructions


  - **d | diff** : Display difference between remote & local
  - **pl | pull** : Pull changes from remote to local
  - **pu | push** : Push changes from local to remote

## Usage
- Begin by creating a config file in the root dircetory using command `syncs -cc`
- Setup the following in the config file:
    - host
    - remote
    - ignore list
- Run `syncs` to display diff between remote and local
- See the above commands list for more info

## TODO
- Sync deleted files/directories
- Sync individual files
- jq installer script
- Add verbose command
