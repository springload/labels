# When creating a new project on GitHub

- Run `npm install -g github-label-sync`
- Make sure you have a file `labels.json` at the root of your project. If you don't, help yourself here:
https://github.com/springload/labels/blob/master/labels.json
- Then make sure you run your terminal at the root of your project
- Then run `github-label-sync --access-token XXXXXXX springload/YOUR_PROJECT`
- You should get an output similar to this:
```
Syncing labels for "springload/springtunes"
Fetching labels from GitHub
 > Missing: the "★★★" label is missing from the repo. It will be created.
 > Missing: the "★★☆" label is missing from the repo. It will be created.
 > Missing: the "★☆☆" label is missing from the repo. It will be created.
 > Missing: the "0 - Backlog" label is missing from the repo. It will be created.
 > Missing: the "1 - Ready" label is missing from the repo. It will be created.
 > Missing: the "2 - Working" label is missing from the repo. It will be created.
 > Missing: the "3 - To be tested" label is missing from the repo. It will be created.
 > Missing: the "4 - Testing" label is missing from the repo. It will be created.
 > Missing: the "5 - Tested" label is missing from the repo. It will be created.
 > Missing: the "6 - Live" label is missing from the repo. It will be created.
 > Missing: the "BED" label is missing from the repo. It will be created.
 > Missing: the "Big" label is missing from the repo. It will be created.
 > Changed: the "bug" label in the repo is out of date. It will be updated to "Bug" with color "#fc2929".
 > Missing: the "Content Update" label is missing from the repo. It will be created.
 > Missing: the "Design" label is missing from the repo. It will be created.
 > Changed: the "duplicate" label in the repo is out of date. It will be updated to "Duplicate" with color "#cccccc".
 > Changed: the "enhancement" label in the repo is out of date. It will be updated to "Enhancement" with color "#84b6eb".
 > Missing: the "FED" label is missing from the repo. It will be created.
 > Missing: the "Future" label is missing from the repo. It will be created.
 > Changed: the "help wanted" label in the repo is out of date. It will be updated to "Help wanted" with color "#cc317c".
 > Changed: the "invalid" label in the repo is out of date. It will be updated to "Invalid" with color "#e6e6e6".
 > Missing: the "Medium" label is missing from the repo. It will be created.
 > Missing: the "Feature name 1" label is missing from the repo. It will be created.
 > Changed: the "question" label in the repo is out of date. It will be updated to "Question" with color "#cc317c".
 > Missing: the "Small" label is missing from the repo. It will be created.
 > Missing: the "Tested & Failed" label is missing from the repo. It will be created.
 > Missing: the "Tested & Passed" label is missing from the repo. It will be created.
 > Missing: the "Won't fix" label is missing from the repo. It will be created.
 > Added: the "wontfix" label in the repo is not expected. It will be deleted.
Applying label changes, please wait…
Labels updated
```

For more info/config about github-label-sync, have a look at https://github.com/Financial-Times/github-label-sync

Here is a list of our labels and their colors:
##PROJECT STAGE LABELS
- Backlog #ccc
- Ready #ccc
- Working #ccc
- To be tested #ccc
- Testing #ccc
- To deploy #ccc
- Live #ccc

##DEPARTMENT LABELS
- Design #fbca04
- FED #0e8a16
- BED #0000CD

##TASK LABELS

###Default github ones (leave default colors apart from specified)
- Bug
- Enhancement
- Won't fix #000000
- Duplicate
- Help wanted #cc317c (same color than Question)
- Question

###Taken from GMI
- Content update #ffb600
- Future #FFF
- Tested & Failed #e99695
- Tested & Passed #c2e0c6

##PRIORITY LABELS
- One star
- Two stars
- Three stars

###ESTIMATION LABELS
- Small #FFEC8B   (X<33% of a feature)
- Medium #F4A460  (33%<X<66% of a feature)
- Big #A52A2A    (66%<X of a feature)

###FEATURE LABELS (Example from GMI sales tool)
- Module 1 #1E90FF
- Module 2 #1E90FF
- Module 3 #1E90FF
- Module 4 #1E90FF
- Module 5 #1E90FF
- etc. just use #1E90FF for all feature labels
