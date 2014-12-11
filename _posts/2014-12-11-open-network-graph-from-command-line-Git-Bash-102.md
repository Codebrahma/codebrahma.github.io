---
layout: post
title:  "Open github network graph from command line"
categories: git
comments: true
description: Open github network graph from command line Git-Bash-102
tags:
  - git
  - bash
author: Nithin Krishna
handle: "nithinkrishh"
---

Github's [network graph](https://github.com/blog/39-say-hello-to-the-network-graph-visualizer) is one most elegant tools to track your project's progress.

Open the network graph of you current project with this shell script.

Just type _network_.

{% highlight bash %}
function network(){
    url=$(git remote -v | grep origin | awk 'FNR == 2{print $2}')
    sub_path=$(echo ${url##*github.com})
    project_name=$(echo ${sub_path:1} | rev | cut -c 5- | rev)
    project_url=$(echo "https://github.com/${project_name}/network")
    cowsay "I'm taking you to $(echo ${project_url})"
    python -mwebbrowser $(echo ${project_url})
}
{% endhighlight %}

<img src="/images/blog/network.png"  alt="Network graph" style="width: 100%; height:auto;" />

***

With a little more customization.

{% highlight bash %}
function open_url(){
  cowsay "I'm taking you to ${1}"
  python -mwebbrowser $1
}

function gh(){
  url=$(git remote -v | grep origin | awk 'FNR == 2{print $2}')
  sub_path=$(echo ${url##*github.com})
  project_name=$(echo ${sub_path:1} | rev | cut -c 5- | rev)
  open_url "https://github.com/${project_name}/${1}"
}
{% endhighlight %}

{% highlight bash %}
gh # Open repo
gh network # Open network graph
gh pulse # Open repo pulse
gh pulls # Open pull requests
gh branches # Open branch list
gh wiki # Open wiki
{% endhighlight %}
