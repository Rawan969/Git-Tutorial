<h1>My favorite git tips</h1>
<h2>1.Show helpful guides that come with Git</h2>
<p>git help -g</p>
<h2>2.Sync with remote, overwrite local changes</h2>
<p>git fetch origin && git reset --hard origin/master && git clean -f -d</p>
<h2>3.Git reset first commit</h2>
<p>git update-ref -d HEAD</p>
</br>
<h1>10 tips and tricks</h1>
<h2>1.List all the conflicted files</h2>
<p>git diff --name-only --diff-filter=U</p>
<h2>2.Unstaged changes since last commit</h2>
<p>git diff</p>
<h2>3.Show both staged and unstaged changes</h2>
<p>git diff HEAD</p>
<h2>4.Remove branches that have already been merged with master</h2>
<p>git branch --merged master | grep -v '^\*' | xargs -n 1 git branch -d</p>
<h2>5.Create local tag</h2>
<p>git tag <tag-name></p>
<h2>6.See commit history for just the current branch</h2>
<p>git cherry -v master</p>
<h2>7.Get list of all remote references</h2>
<p>git remote</p>
<h2>8.Get list of all local and remote branches</h2>
<p>git branch -a</p>
<h2>9.See all commits made since forking from master</h2>
<p>git log --no-merges --stat --reverse master..</p>
<h2>10.Saving current state with message</h2>
<p>git stash push -m <message></p>
