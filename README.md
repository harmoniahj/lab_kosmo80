# lab_kosmo80
Web레포 시작, 콜라보를 위한 첫 단추
[user]
	name = harmoniahj
	email = harmoniahj@naver.com
[filter "lfs"]
	required = true
	clean = git-lfs clean -- %f
	smudge = git-lfs smudge -- %f
	process = git-lfs filter-process
[core]
	autocrlf = input
	editor = code --wait
[pull]
	rebase = false
[diff]
	tool = vscode
[difftool "vscode"]
	cmd = code --wait --diff $LOCAL $REMOTE
[merge]
	tool = vscode
[mergetool "vscode"]
	cmd = code --wait $MERGED
[alias] hist = log --graph --all --pretty=format:'%C(yellow)[%ad]%C(reset) %C(green)[%h]%C(reset) | %C(white)%s %C(bold red){{%an}}%C(reset) %C(blue)%d%C(reset)' --date=short

