---
title: "Sample Git Configuration"
date: 2019-01-20T18:49:50-05:00
draft: false
---
Git configurations can be pre-configured in this file to specify default editors, aliases, coloring and many other options.  Below is a simple starter configuration
<pre class="aLF-aPX-K0-aPE"><code>
[user]
	name = Your Name
	email = yourEmail@domain.com
[core]
	editor = vim
	whitespace = fix,-indent-with-non-tab,trailing-space,cr-at-eol
	excludesfile = ~/.gitignore
[alias]
	lol = log --graph --decorate --pretty=oneline --abbrev-commit
        lola = log --graph --decorate --pretty=oneline --abbrev-commit --all
[color]
        branch = auto
        diff = auto
        interactive = auto
        status = auto
</code></pre>
