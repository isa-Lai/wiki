# Other Tools

## Git
Git push now no support password, have to use **Token** generated in gitub setting. To push, set this in git bash.
```git
git remote set-url origin https://<your_token>@github.com/<USERNAME>/<REPO>.git
git remote set-url origin https://ghp_sometokencode@github.com/isa-lai/isa-lai.github.io.git/
```

Any wrong SSL verifycation may solve by
```git
git config --global http.sslVerify "false"
```

