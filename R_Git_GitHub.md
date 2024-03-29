<style>
.section .reveal .state-background {
    background: white;}
.section .reveal h1,
.section .reveal p {
    color: black;
    position: relative;
    top: 1%;}
    </style>
    
<style>

.footer {
    color: black; background: white;
    position: fixed; top: 100%;
    text-align:left; width:100%;
}

</style>


R is to RStudio as Git is to GitHub 
========================================================
author: Cory Whitney   (cory.whitney@uni-bonn.de)
font-family: 'Helvetica'
autosize: true
css: mySlideTemplate.css
<img src="R_Git_GitHub-figure/github.png" style="background:none; border:none; box-shadow:none;height="400"; width="400";"><img src="R_Git_GitHub-figure/INRES_Logo.png" style="background:none; border:none; box-shadow:none;height="100"; width="100";"><img src="R_Git_GitHub-figure/Uni_Bonn_Picture.png" style="background:none; border:none; box-shadow:none;height="200"; width="200";"><img src="R_Git_GitHub-figure/ZEF_Logo.png" style="background:none; border:none; box-shadow:none;height="200"; width="200";">

Automated version control
========================================================
incremental: true

**Never have I ever:**
- used 'cmd z' or 'ctrl z'
- came to the office but left the work at home on another machine or USB
- tried to co-author scripts by emailing files back and forth

<small>**Git** is an open source version control tool, **GitHub** is a company that hosts Git repositories in the web and provides a web interface to interact with repos they host.</small>

***

![](R_Git_GitHub-figure/final_doc_comic.png)

<div class="footer" style="margin-top;font-size:60%;"> 
https://swcarpentry.github.io/git-novice/guide </div>

Git: overview
========================================================
incremental: true
right: 80%
![](R_Git_GitHub-figure/git_logo.png)
<small>https://git-scm.com/</small>

***

A better way to:
- "undo" changes,
- collaborate than mailing files back and forth, and
- share code and other scientific work with the world.

<img src="R_Git_GitHub-figure/git_logo_orange.png" title="plot of chunk unnamed-chunk-1" alt="plot of chunk unnamed-chunk-1" width="35%" style="display: block; margin: auto;" />

<div class="footer" style="margin-top;font-size:60%;"> 
<https://swcarpentry.github.io/git-novice/guide> </div>

GitHub: overview
========================================================
incremental: true
right: 80%
![](R_Git_GitHub-figure/octocat.png)

***

your local repository consists of three "trees" maintained by git. the first one is your `Working Directory` which holds the actual files. the second one is the `Index` which acts as a staging area and finally the `HEAD` which points to the last commit you've made.


***

<img src="R_Git_GitHub-figure/git_areas.jpg" title="plot of chunk unnamed-chunk-2" alt="plot of chunk unnamed-chunk-2" style="display: block; margin: auto;" />

<div class="footer" style="margin-top;font-size:60%;"> http://rogerdudler.github.io/git-guide/ </div>

Git and GitHub: getting stuck
========================================================
incremental: true
right: 80%
![](R_Git_GitHub-figure/octocat.png)
***

- If you get stuck, just add “Git” to a search query e.g. a short description of your issue
- Someone else has also been confused by it and has written about it
- Thousands of talented programmers who scan the web and answer these problems
<img src="R_Git_GitHub-figure/stack-overflow.png" title="plot of chunk unnamed-chunk-3" alt="plot of chunk unnamed-chunk-3" width="50%" style="display: block; margin: auto;" />

<div class="footer" style="margin-top;font-size:60%;"> 
https://stackoverflow.com/ </div>

Git and GitHub: basics
========================================================
incremental: true
right: 80%
![](R_Git_GitHub-figure/octocat.png)
***

Install Git & join Github (if you have not already):

- install Git
<small>https://git-scm.com/downloads</small>

- join Github
<small>https://github.com/</small>


Some useful tips on getting these running from our friends 

- University of Zurich
<small>http://www.geo.uzh.ch/microsite/reproducible_research/post/rr-rstudio-git/</small>

- Nathan Stephens, a very helpful R blogger 
<small>https://support.rstudio.com/hc/en-us/articles/200532077-Version-Control-with-Git-and-SVN</small>

GitHub: host for your code
========================================================
incremental: true
right: 80%
![](R_Git_GitHub-figure/octocat.png)
***
**GitHub** 
- a commercial website that lets you store repository publicly for free [get an education account with an uni email address](https://help.github.com/en/articles/applying-for-an-educator-or-researcher-discount)
- a friendly interface, no need to remember command line. 
- useful features including issues, wikis etc.

<img src="R_Git_GitHub-figure/Github-Icon-4.png" title="plot of chunk unnamed-chunk-4" alt="plot of chunk unnamed-chunk-4" style="display: block; margin: auto;" />

GitHub: intro hello-world
========================================================
incremental: true

![plot of chunk unnamed-chunk-5](R_Git_GitHub-figure/Hello_world.jpg)

<small>https://guides.github.com/activities/hello-world/</small>

Git: Command line
========================================================
incremental: true
right: 80%
![](R_Git_GitHub-figure/git_logo.png)
<small>https://git-scm.com/</small>
![](R_Git_GitHub-figure/git_logo_orange.png)

***

- `git reset --soft HEAD~1` or `commit SHA` 
we undo our last commit, but the changes contained in that commit are not lost

- `git reset --hard HEAD~1` or `commit SHA`
we discard all changes we've made in the working directory 

- `git stash`  
move the waiting changes out of the queue

<div class="footer" style="margin-top;font-size:60%;"> 
https://jennybc.github.io/2014-05-12-ubc/ubc-r/session03_git.html </div>

