# Using multiple ssh-keys

Steps:
- Clone your project repo.
- Set the username and email: \
`git config user.name` \
`git config user.email`
- Set the `core.sshCommand` attribute as: \
`git config core.sshCommand "ssh -i ~/.ssh/id_your_key"`

