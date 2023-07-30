# Using multiple ssh-keys

Steps:
- Clone your project repo.
- Set the username and email: \
`git config user.name` \
`git config user.email`
- Set the `core.sshCommand` attribute as: \
`git config core.sshCommand "ssh -i ~/.ssh/id_your_key"`


Or if you're on a windows machine, add the following code after changing the relevant parts to your Powershell profile. \
To access the powershell profile, open a terminal window with powershell and enter the command: `notepad $profile` \
You can use any text editor you have installed. For example  `code $profile` for VS Code, or `nvim $profile` for neovim.



Add the following powershell function to the end of the file.

```powershell
Function Set-LocalGit{
  git config user.name "your name"
  git config user.email "your email"
  git config core.sshCommand "ssh -i ~/.ssh/id_yourkey"
}
```


Refresh the profile with `. $profile` \
Now you can set these defaults in any local repo using the powershell function `Set-LocalGit`

Cheers!