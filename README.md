# Git Tricks - a Github and Git Reference

# Contents
[Git - Setup Default User Info](#git-user-info) <br>
[Git - Setup Proxy](#git-proxy) <br>
[Github MD - Code Blocks](#github-code) <br>
[Official Github .gitignore Templates](#gitignore) <br>



<a id="gitignore"></a>
## Official Github .gitignore Templates
<a id="gitignore-link">https://github.com/github/gitignore</a>


<a id="git-user-info"></a>
## Set your default Github user information in Git
- use the same email that you have registered to Github
- can be `--global` or `--local`

`git config --global user.name <name>`
<br>
`git config --global user.email <email>`


<a id="git-proxy"></a>

## How to use Git with a proxy

Set: <br>
`git config --global http.proxy http://proxyuser:proxypwd@proxy.server.com:8080`
<br>
`git config --global https.proxy https://proxyuser:proxypwd@proxy.server.com:8080`

Get: <br>
`git config --global --get http.proxy`

Unset: <br>
`git config --global --unset http.proxy`


### Global:
To commit and checkout line endings globally as you saved them:
<br>
`git config --global core.autocrlf false`

To checkout as your OS line endings (CRLF Windows, CR Unix) and commit as Unix
<br>
`git config --global core.autocrlf true`


### Local
Create a `.gitattributes` file and enter the setting you need for the repo.  You can also specify files/filetypes
- `* text=auto`
- `* text eol=crlf`
- `* text eol=lf`


<a id="github-code"></a>

## Github Markdown - Code Blocks

- Inline code enclosed by tick marks  ( \` )

  Example: `inline code`

- Block code with triple tick marks ( \`\`\` )

  Example:
  ```
  Block Code
  Place tick marks on separate lines
  ```

- escape a tick mark in inline code by using 2 tick marks to enclose the code
- escape a tick mark in block code by using 4 tick marks to enclose the code

- you can specify programming language to get highlighted syntax by placing langugage name next to first \`\`\` marks

  List of supported syntax: https://github.com/github/linguist/blob/master/vendor/README.md 

  Python Example:
  
  ````
  ```python
  x = 10
  def main()
  ```
  ````
  
  ```python
  x = 10
  def main()
  ```
