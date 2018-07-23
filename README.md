# Git Tricks - a Github and Git Reference

### Set your default github user information
- use the same email that you have registered to Github
- can be `--global` or `--local`

`git config --global user.name <name>`
`git config --global user.email <email>`

Local:

### How to use Git with a proxy

Set:
`git config --global http.proxy http://proxyuser:proxypwd@proxy.server.com:8080`
`git config --global https.proxy https://proxyuser:proxypwd@proxy.server.com:8080`

Get:
`git config --global --get http.proxy`

Unset:
`git config --global --unset http.proxy



