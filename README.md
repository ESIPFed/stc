# Repository for the ESIP Semantic Technologies Committee

<img src="http://www.esipfed.org/sites/default/files/esip-logo.png" align="right" width="300" />
<a href="http://esipfed.org">![](http://badge.esipfed.org/testbed.svg?display=logo)</a> 
<a href="http://esipfed.org">![](http://badge.esipfed.org/semanticweb.svg?display=logo)</a>

**All Committee Working, Editors DRAFT's and Official documents are linked to from the [Website](https://esipfed.github.io/stc/)**

# How to work with us on Github
The following is a recommended ESIP STC Github workflow for collaborative document drafting:
 1. create a local copy of the ESIPfed STC repo ```git clone https://github.com/esipfed/stc.git```
 2. configure remotes on local - specify the ESIPfed STC repo remote as 'upstream': ```git remote add upstream https://github.com/esipfed/stc.git```
 3. fetch the branches and their respective commits from the upstream repository: ```git fetch upstream```
 4. because we're using [GitHub Pages](https://pages.github.com/) for publication, `gh-pages` is our main branch
 5. log an issue in the [stc issue tracker](https://github.com/ESIPFed/stc/issues).  Please use [labels](https://help.github.com/articles/applying-labels-to-issues-and-pull-requests/) to classify your issue. If you need a new label to be created then please state this in your issue description. 
 6. create a branch in your local repo which tracks gh-pages in upstream. The branch name should reflect the issue number you created above e.g. [STC-1](https://github.com/ESIPFed/stc/issues/1) ```git checkout -b STC-1 upstream/gh-pages```
 7. make the changes in your branch & commit - with commit message please! e.g. ```git commit -m "STC-1 Clarify reference to Ontology Repositories as 'Semantic repository implementation' (SRI)"```
 8. synchronise your changes with upstream: ```git push upstream STC-1```
 9. now would be a good time to [format](http://www.freeformatter.com/html-formatter.html) (2 space indents please) and [validate](https://validator.w3.org/) your HTML if you intend to include it within your pull request.
 10. within GitHub, create a Pull Request from STC-1 into gh-pages ... at this point, you might assign the Pull Request to someone else to check before merging
 11. **EDITORS ONLY**: within GitHub, Merge the changes into gh-pages ... then you will see the new commit version linked to and available from http://esipfed.github.io/stc
 12. bring all those changes back into your local repo: ```git fetch upstream```
 13. rebase (don't 'pull' - because this creates another commit) changes on your branch: ```git rebase upstream/gh-pages```

(you might also want to rebase local/gh-pages too)

Alternatively - send your text to the Editors via the [WG email list](http://lists.esipfed.org/mailman/listinfo/esip-semanticweb). 
