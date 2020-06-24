# gitconfing 設定

```bash
git config --system alias.s status
git config --system alias.st status
git config --system alias.pl pull
git config --system alias.p pull
git config --system alias.co checkout
git config --system alias.b branch
git config --system alias.br branch
git config --system alias.cm commit
git config --system alias.ps push
git config --system alias.unstage reset HEAD
git config --system alias.ft fetch
git config --system alias.gr = log --graph --date=short --decorate=short --pretty=format:'%Cgreen%h %Creset%cd %Cblue%cn %Cred%d %Creset%s'
git config --system alias.dp = diff --no-prefix
git config --system alias.dsp = diff --cached --no-prefix
git config --system alias.log --pretty='format:%C(yellow)%h%Creset %C(magenta)%cd%Creset %s %Cgreen(%an)%Creset %Cred%d%Creset%C(black bold)%ar%Creset' --date=iso
git config --system alias.lga = !"git lg --all"
git config --system alias.sgraph = !"git log --oneline --graph"
git config --system alias.ancestor = !zsh -c 'diff -u <(git rev-list --first-parent "${1:-master}") <(git rev-list --first-parent "${2:-HEAD}") | sed -ne \"s/^ //p\" | head -n 1' -
git config --system alias.cp = cherry-pick
git config --system alias.bg = log --graph --simplify-by-decoration --pretty=format:'%d' --all
git config --system alias.today = log --oneline --since='12 hour ago'
```
