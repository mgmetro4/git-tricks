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



