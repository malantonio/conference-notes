git bisect: worked at x commit, doesn't work at z commit, go through and find out what went wrong

git rebase??
- backs up to point of branching, fast-forwards to HEAD and applies branch commits ( no wavy branch lines )
- _cleaner_
- can squish multiple commits into one (using -i interactive mode, 'squash') ( helpful w/ contributing to open source projects )

git blame
- file w/ blame attached line-by-line

'pickaxe'
git log -S <search term>

commit + tilde + number back => show number of commits before

git reset
--soft is default: moves back to previous commit, leaves files unstaged
--hard effectively removes changes

fast-forward merge
- branch merged into is one commit behind merging branch


git mergetool to help w/ merge conflicts ( opendiff, add to config )