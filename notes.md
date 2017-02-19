
git@github.com:emeraldjava/minimal-mistakes.git


git-workflow

http://stackoverflow.com/questions/4750520/git-branch-gh-pages
https://gist.github.com/chrisjacob/833223/923ed1312291ee84450b99b9433335174404eba2

https://gist.github.com/chrisjacob/825950

https://gist.github.com/cobyism/4730490

http://stackoverflow.com/questions/6270193/multiple-working-directories-with-git/30185564#30185564


```
git checkout -b gh-pages

git worktree add gh-pages gh-pages
```

from http://pressedpixels.com/articles/deploying-to-github-pages-with-git-worktree/

```
git reset
git commit --allow-empty -m 'Initial commit'
git checkout --force master
git worktree add dist gh-pages
```

this gives

```
pauloconnell@pauloconnell-HP-ZBook-15 ~/projects/github/minimal-mistakes $ git worktree list --porcelain
worktree /home/pauloconnell/projects/github/minimal-mistakes
HEAD 77db91ad4f6bf818ffe3b1e7ee072882ee3592ef
branch refs/heads/master

worktree /home/pauloconnell/projects/github/minimal-mistakes/gh-pages
HEAD 641854267a33e1a7a0b999e7c515dccda1d742b5
branch refs/heads/gh-pages
```

git remote set-url origin git://github.com:emeraldjava/minimal-mistakes.git

https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/

```
/github/minimal-mistakes/gh-pages $ rm -rf .editorconfig 
/github/minimal-mistakes/gh-pages $ rm -rf .gitattributes 
/github/minimal-mistakes/gh-pages $ rm -rf .github
/github/minimal-mistakes/gh-pages $ rm -rf docs
/github/minimal-mistakes/gh-pages $ rm -rf test
/github/minimal-mistakes/gh-pages $ rm -rf CHANGELOG.md 
/github/minimal-mistakes/gh-pages $ rm -rf minimal-mistakes-jekyll.gemspec 
/github/minimal-mistakes/gh-pages $ rm -rf README.md 
/github/minimal-mistakes/gh-pages $ rm -rf screenshot-layouts.png 
/github/minimal-mistakes/gh-pages $ rm -rf screenshot.png 
```

https://emeraldjava.github.io/minimal-mistakes/