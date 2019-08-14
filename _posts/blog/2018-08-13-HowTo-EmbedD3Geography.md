---
layout: post
title: "How To: Embed D3 Geographies (Maps)"
modified:
categories: blog
excerpt:
tags: [Guide]
date: 2018-08-13T15:39:55-04:00
---

This guide shows the steps into incorporating d3 visualization into your Github page. 

### Step 1: Create script

For example scripts and visualization, you can visit the [d3 gallery](https://github.com/d3/d3/wiki/Gallery){:target="_blank"} for ideas. 
Earlier version of d3 visualizations found on this website is coded with version 3. I will be updating most d3 to utilize version 5 (and newer version when they come out). 

You can tell which version of d3 was used by looking at the source code for the script import section, where:

    version 3:
    <script src="https://d3js.org/d3.v3.min.js"></script>

    version 5:
    <script src="https://d3js.org/d3.v5.min.js"></script>

Most of my scripts will be in the **index.html** file. 

### Step 2: Testing locally

cd into your folder with the index file and type: 

    python -m SimpleHTTPServer

This will serve your website on localhost on port 8000 where you can view your d3 website locally. 

In your browser, to view, copy and paste: 

    http://localhost:8000/

### Step 3: Push to Gist

[Gist](https://gist.github.com/){:target="_blank"} is a Github feature. 
It allows you to share parts of files easily. But with html files, we can utilize gist as a starting point to a view of the website from other sources.
First you want to upload your **index.html** files and any data files that it uses onto gist. Each "gist" is its own repository. Also note the difference between
 "secret gist" and "public gist". Secret gist are not searchable but you can share the link with other people, whereas public gist can be searched by the public. 
For more information about gist, click [here](https://help.github.com/articles/about-gists/){:target="_blank"}.

For this example, I have created a gist at:
<font color="blue">https://<font color="red">gist.github.com</font>/vincentpham1991/bdde5f0ad54449717bacbf75b6eeee96</font>

### Step 4 (optional): Visualize the gist

replace **gist.github.com** from step 3 with **bl.ocks.org** from your gist. 

<font color="blue">https://<font color="red">bl.ocks.org</font>/vincentpham1991/bdde5f0ad54449717bacbf75b6eeee96</font>

This will allow you to get a visual view of the index file you placed in your gist. It should be the same as what you see in step 2, but allows for a non-local solution in case
you do minor changes directly to your gist.


### Step 5: get embedding of gist (deprecated)

**RAWGIT is going offline in October 2019**

From the gist, click on **Raw** for the index file. Copy the url. in this case it would be:
<font color="blue">https://gist.githubusercontent.com/vincentpham1991/bdde5f0ad54449717bacbf75b6eeee96/raw/47c6095c9085cc99d6dbbc7e7887ace1b004abb9/index.html</font>

go to **rawgit.com**

paste the url where it tells you to. 

This will give you links that you can use to post d3 on your Github page. Choose the one that best suites your case:

production url: <font color="blue">https://cdn.rawgit.com/vincentpham1991/bdde5f0ad54449717bacbf75b6eeee96/raw/47c6095c9085cc99d6dbbc7e7887ace1b004abb9/index.html</font>
development url: <font color="blue">https://rawgit.com/vincentpham1991/bdde5f0ad54449717bacbf75b6eeee96/raw/47c6095c9085cc99d6dbbc7e7887ace1b004abb9/index.html</font>

### Step 6: Embed link into Github page (deprecated)

This step may be different depending on the method you use to create your Github page. But for me, I can host it by using this line: 


<font color="red"> 
<iframe width="1000" height="600"    
src="https://rawgit.com/vincentpham1991/bdde5f0ad54449717bacbf75b6eeee96/raw/47c6095c9085cc99d6dbbc7e7887ace1b004abb9/index.html"         
...
</font> 
    
