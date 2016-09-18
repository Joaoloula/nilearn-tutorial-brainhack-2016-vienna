# Nilearn tutorial for brainhack 2016 at Vienna

## When?

The tutorial will take place on Monday, 19th at 11 in Jugendstilhörsaal.

## Preparing your computer for the tutorials

No action is required during the tutorial: We will explain the code and present
the results. There will be an online version that you can easily follow.
However, we strongly encourage you to run the example on your computer, just as
we speak.

### Installing nilearn

Follow the instructions on the nilearn
website.

http://nilearn.github.io/introduction.html#installing-nilearn

### Downloading the data for the tutorial

First, you need to start ipython. Just type `ipython` in your terminal. Then,
copy paste the following lines:

```python
from nilearn.datasets import fetch_abide_pcp

fetch_abide_pcp(derivatives='func_preproc', n_subjects=3, SITE_ID=['NYU'],
                pipeline='cpac')
fetch_abide_pcp(derivatives=['rois_cc200'], SITE_ID=['NYU'], pipeline='cpac')
```

### Downloading extra data

We will show the result of a full analysis on ABIDE. You do not have to run it
yourself but, if you want to do it, you will need the timeseries of all ABIDE
subjects. Run the command below (after the others) to download them.

```python
fetch_abide_pcp(derivatives=['rois_cc200'], pipeline='cpac')
```
