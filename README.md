# Using multiple ssh-keys

Steps:
- Clone the repo
- Set the username and email: \
`git config --local user.name` \
`git config --local user.email`
- Edit the config file for the local repo  \
`git config --local --edit`
- In the [core] section, add sshCommand using the location of the preferred ssh-key. \
Eg. `sshCommand=ssh -i ~/.ssh/id_rsa_test` \
Or set it using the following command. \
`git config --local core.sshCommand=ssh -i ~/.ssh/id_rsa_test`
