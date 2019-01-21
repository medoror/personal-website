---
title: "Useful Unix Commands"
date: 2019-01-20T19:03:33-05:00
draft: false
---
Miscellaneous post.  Using Unix from time to time for administrative tasks.  Below is a running log of useful Linux commands that I always forget



Search for keywords in a file

<code> find . -type f -name "file" | xargs grep "keyword" </code>

Find largest files over 100M in filesystem

<code> find / -xdev -type f -size +100M -exec ls -la {} \; | sort -nk 5 </code>
