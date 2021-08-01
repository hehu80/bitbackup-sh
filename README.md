# Bitbackup

## Description
This bash script will download all of your Git repositories from a Bitbucket workspace.
If a repository does not exist locally the repo will be cloned to the target directory. If a
repository already exists locally, `git remote update` will be run.


## Usage
```bash
bitbackup -k <bitbucket app key> -u <bitbucket username> -w <bitbucket workspace> 
  [-t <target directory>] [-p <bitbucket projectname>]
```
_App Key_ and _Username_ a required to access the Bitbucket API. You can easily generate a new App Key
at your personal [settings page](https://bitbucket.org/account/settings/app-passwords/) in Bitbucket.
_Workspace_ could be your own _username_ to download your personal repositories or one of the team workspaces.
To download only repositories of a certain project, you can specify the _project name_.