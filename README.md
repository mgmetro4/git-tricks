# Git Tricks - a Github and Git Reference

### Set your default Github user information
- use the same email that you have registered to Github
- can be `--global` or `--local`

`git config --global user.name <name>`
<br>
`git config --global user.email <email>`


### How to use Git with a proxy

Set: <br>
`git config --global http.proxy http://proxyuser:proxypwd@proxy.server.com:8080`
<br>
`git config --global https.proxy https://proxyuser:proxypwd@proxy.server.com:8080`

Get: <br>
`git config --global --get http.proxy`

Unset: <br>
`git config --global --unset http.proxy`

### Line Endings
#### Global:
To commit and checkout line endings globally as you saved them:
<br>
`git config --global core.autocrlf false`

To checkout as your OS line endings (CRLF Windows, CR Unix) and commit as Unix
<br>
`git config --global core.autocrlf true`


#### Local
Create a `.gitattributes` file and enter the setting you need for the repo.  You can also specify files/filetypes
- `* text=auto`
- `* text eol=crlf`
- `* text eol=lf`

