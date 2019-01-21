---
title: "Git Workflow"
date: 2019-01-20T18:38:18-05:00
draft: false
---
General steps for working with projects in GitHub
<ol>
 	<li>Use the graphical UI on Github and fork the repository.</li>
 	<li>Clone the forked repo to local computer:
<code>git clone https://github.com/&lt;user_name&gt;/&lt;repository&gt;.git</code></li>
 	<li>Create an upstream remote to your remote repository:
<code>cd &lt;repository&gt;</code>
<code>git remote add upstream https://github.com/&lt;remote-repository-path&gt;.git</code></li>
 	<li>Create a local branch for the current feature:
<code>git checkout -b &lt;user_name&gt;/&lt;issue&gt;</code></li>
 	<li>Make commits to your local master branch:
<code>git commit -a</code></li>
 	<li>Make sure you leave a detailed commit message</li>
 	<li>Pull from upstream master using rebase and resolve conflicts:
<code>git pull --rebase upstream &lt;user_name&gt;/&lt;issue&gt;</code></li>
 	<li>Push to your fork's feature branch:
<code>git push origin &lt;user_name&gt;/&lt;issue&gt;</code></li>
 	<li>Create Pull request to the repositories master branch of the repository.  Make sure you leave a detailed message</li>
</ol>
<a href="http://michaeledoror.com/wp-content/uploads/2017/08/GitWorkflow-3.png"><img class="alignnone size-full wp-image-256" src="http://michaeledoror.com/wp-content/uploads/2017/08/GitWorkflow-3.png" alt="" width="748" height="561" /></a>
