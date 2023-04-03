- When you're at the step of trying to push your local to your remote by typing.

```bash
git push -u origin master
```

- Esto me parece que pasa es cuando se trata de hacer un push a un repositorio privado

You'll encounter an error since you need to create a personal access token and enter that instead of your git password.

You cannot use your password for `git push` or other Git operations (but you still need it to log in). You need to [create a personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) and enter that instead when Git asks for your password. When creating the token make sure to select the **repo** scope (for repository access, like pushing) and if you use Actions also **workflow** (required to modify workflow files).

https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token

- Tiene que generar un token y darle permisos de escritura.
