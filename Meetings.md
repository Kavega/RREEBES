# Meetings in 2015

Meetings 10.45 to 12.00 Zurich time, location is variable.

Assign person to take meeting minutes.

New people (get photo)?

Any suggested papers added to the repository?

Any outstanding issues?

Any progress on focal paper since last week?

What to attempt this week (refer to closing note from last week)?

What to attempt next week (to be refered to next week)?

## 3.3

(Minutes by Mikael.)
Owen introduced and outlined REEBBES by going through the GitHub homepage
* How to suggest papers to reproduce
* Meeting schedule
* Potential papers to reproduce
* How to contribute at meetings or outside the meeting schedule
    -State issues on the Github webpage
    -Get an account on Github and edit files

How to make a report in r-studio (see e.g. report in the folder RREEBES/Beninca_etal_2008_Nature on Github)

Owen introduced the Beninca et al 2008 data.
* The raw data is available in a xls-file, available on Github
    -Species abundance and nutrient concentrations are available
    -The data that will be used for the reproduction in R is provided as csv-files, also on Github.
 
Get started with the reproduction in R (see also report in REEBES/Beninca_etal_2008_Nature on Github)
* Import the csv files into R-studio and clean up data.

Frank introduced how to get on Github and to clone info. between Github and your local computer
* Get an account and log in
* Clone by clicking on the fork-button
* Clone to your local computer by copying the URL to your computer

## 10.3

(Minutes by Marco.)
Recap for those that missed the previous meeting:
* what are git and github, what is version control;
* how to keep an eye on a github repository by using the “watch” option;
* using github desktop app for managing repositories.

Homeworks for next time:
* create a github account
* find the RREEBES repository and follow its changes and developments using the “watch” option
* try to make a change to one of the existing files and make a “pull” request

## 17.3

(Minutes by Vanessa.)
New people: Gian Marco

Suggestions
* Email the authors of the papers that we start to reproduce, let them know what we are doing and where the files will be available.

Questions
* Owen and Frank showed how to properly fork and clone the repository into your own account/computer, how to edit the files and then pull them back. Thiss will be available on the wiki page.

Issues
* Jason: what kind of paper we are interested in reproducing, and also which analyses within a paper we would like to reproduce.
* How to read data from github

No progress since last week

Continue to work on the Beninca et al 2008 paper:
* Reproduce fig. 1
* Generated figure is similar to the original one in the paper, but not exactly the same. Is this enough? Do we need to reproduce exactly the same plot?

Next week: go through the modifications sent by Owen


## 24.3

Owen not present.
No meeting.

## 31.3

Owen not present.
No meeting.

## 7.4

Owen not present.
No meeting.

## 14.4

(Minutes by Gian Marco.)

* Owen encourages to meet even in his absence.
* Vanessa has troubles synchronising the github ?> instructions on the wiki.
* Some of us have troubles connecting to the internet ieu Petchey ?> Go to IT to unlock the network.

* Work on the master branch.
* Issue: use package RCurl function getURL to read the file from the internet.
* Recap of previous work done on the Beninca paper.

* Change branch to Figs2b g.
* Fix some details (names of data and variables) in the current branch.
* Check of previous plot of time series.
* Create a color map for the species adding colours to different functional groups.
* Reproduce color figure without magnifications and gaps.
* Try to approximate the gap by removing the data above a given value.
* Plot log scale and fourth root plots.

* Go back to master branch and synchronise.
* Todo for next week: data transformation and Lyapunov exponents.
* Jason shows reproduction of Hiltunen et al. (2014).

## 21.4

(Minutes taken by Frank)

#### Organization:

* no new papers or faces
* change the working of RREEBES: groups (e.g. 2 persons) work in parallel rather than watch Owen code; Tuesdays to present progress and work on specific issues that appeared during group work

##### Continuation reproducing Beninca et al. 2008:

Getting data ready for analysis:

1. interpolation
	* no cubic hermite interpolation function in R, so we use spline to get time points with equidistance of 3.35 days (see open issue)
	* spline -> provides various methods, we are not sure which may be the exact corresponding method but hopefully it should not matter too much for following analysis; potential alternative package pracma

	* interpolations look mostly reasonable, but seems strongly affected by NAs in the data; funky shapes that go below zero for some species

2. transformation 
	* use fourth square root transform to get rid of sharp spikes
	* some question whether we should do the transformation before the interpolation: in Beninca et al, it is done after interpolation, but we do it before

3. Detrending
	* detrending the data with gaussian kernel (function ksmooth())

4. Scaling
	* re-scaling data to mean 0 and SD of 1


**We are now ready analyze the data (y variable in dataset final)**


#### Distributing tasks for next meeting:

* spectral analysis: Jason, Frank
* table: Kevin, Marco
* Lyapunov (direct): Gian-Marco, Mikael
* Lyapunov (indirect): Vanessa, Dennis

Some material collected by Owen to assist with analyses found here: /Beninca_etal_2008_Nature/report/material_to_use



## 28.4

## 5.5

## 12.5

## 19.5

## 26.5

## 2.6

## 9.6

## 16.6

## 23.6

## 30.6

## 7.7

## 14.7

## 21.7

## 28.7

## 4.8

## 11.8

## 18.8

## 25.8

## 1.9

## 8.9

## 15.9

## 22.9

## 29.9

## 6.10

## 13.10

## 20.10

## 27.10

## 3.11

## 10.11

## 17.11

## 24.11

## 1.12

## 8.12

## 15.12

## 22.12
