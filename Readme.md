# DCManager
A dev container to manage other dev containers specially with named volumes.

### Usage
- Assuming you have a named volume qclose-repos available with multiple repos cloned inside it
- Clone this Repo somewhere else
- Create Dev Container from it (qclose-repo will be mounted at /workspaces)
- To create dev container based on any folder available inside it, run `devcontainer up --workspace-folder <name-of-folder>`
- Once done, new dev container will start showing up in Dev Containers vscode extension, click on 'Open in container in new window' against its name.

### Notes
If file permissions cause issue, ownership of the whole folder can be taken as `sudo chown -R node .` where node is the name of user (being used in most of our node based dev containers)