---
title: "Git Cheat Sheet"
date: 2019-01-20T18:31:07-05:00
draft: false
---

Git is absolutely essential knowledge if you want to be a developer. If you don't know get <a href="/should-i-use-git/">familiar</a>. For more of my take on git workflow and configurations see my other post. Below is my personal cheat sheet and useful commands I have come across

&nbsp;

&nbsp;
<p style="text-align: center;"><strong>Useful Commands</strong></p>
Create a branch and switch to it with local changes

<code>git checkout -b &lt;branch-name&gt; origin/&lt;branch&gt;</code>

Push created feature branch to the remote

<code>git push -u origin &lt;branch-name&gt;</code>

Squash commits

<code>git rebase -i HEAD~&lt;number of commits to squash&gt;</code>

Grabs a commit from another branch

<code>git cherry-pick &lt;SHA&gt;</code>

Add all untracked files

<code>git add -A</code>

Commit all files

<code>git commit -a</code>

Fix commit message or commit

<code>git commit --amend</code>

Useful commit to grabbing a range of commits to place into current branch using a recursive strategy. Strategies can be used for git merges and pulls.  More info can be found here

<code>git cherry-pick --strategy=recursive -X theirs &lt;oldest-sha-included&gt;^..&lt;newest-sha&gt;</code>

[caption id="attachment_88" align="alignnone" width="1753"]<img class="size-full wp-image-88" src="http://michaeledoror.com/wp-content/uploads/2017/08/Git-Cheat-Sheet-pdf-v2.png" alt="https://zeroturnaround.com/wp-content/uploads/2016/02/Git-Cheat-Sheet-pdf-v2.png" width="1753" height="1240" /> https://zeroturnaround.com/wp-content/uploads/2016/02/Git-Cheat-Sheet-pdf-v2.png[/caption]