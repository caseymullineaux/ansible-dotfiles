# antible-dotfiles
Inspired by: 
- https://github.com/TechDufus/dotfiles
- https://github.com/ALT-F4-LLC/dotfiles

## vault-password.txt
The `vault-password.txt` file is used to store the password for the ansible vault, which allows you to encrypt and decrypt files in the repository. This file should be placed in the root of the repository and should contain the password for the vault on the first line of the file.

```bash
vim vault-password.txt
```

To encryt values with your vault password, use the following command:

```bash
ansible-vault encrypt_string --vault-password-file $HOME/.config/dotfiles/vault-password.txt 'mysupersecretvalue' --name 'MY_SECRET_VAR'
```

Alternatively, you can the contents of a file with the following command:

```bash
cat ~/.ssh/id_rsa | ansible-vault encrypt_string --vault-password-file $HOME/.config/dotfiles/vault-password.txt --stdin-name "id_rsa"
```


. It is not included in the repository for security reasons.


## To Do:
### Mac
- brew install zsh-syntax-highlighting
- brew install zsh-autosuggestions
- brew install wezterm
- brew install --cask hyperkey
- brew install eza
- brew install fzf

Aliases:

