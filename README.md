# trouble-shooting-git
Unable to ignore .terraform before pushing to GitHub

Refer Blog: 
1) https://blog.gitguardian.com/rewriting-git-history-cheatsheet/
2) https://github.com/hashicorp/terraform-guides/issues/92

git filter-branch -f --index-filter 'git rm --cached -r --ignore-unmatch .terraform/'
