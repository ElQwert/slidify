---
title       : Image Classification
subtitle    : Model evaluation
author      : Andrey
job         : Data Scientist
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Project description

Classification model was created to classify images - bad/good automatically. 
<br><br>
This application helps to assess model performance. It contains results of 405 models. First result is based on 2 images in training set and next results gets by incrementing number of images by 1.
<br><br>
Final model result based on 406 images in training set.


--- .class #id 

## Performance Metrics of final model





```
## Accuracy:  0.9009901
```

```
## TP:  44  FP:  4  FN:  6  TN:  47
```

```
## Precision:  0.9167  Recall:  0.88  F1 Score:  0.898
```

--- .class #id 

## Learning curves

By plotting learning curves we can assess how does the accuracy of a learning method change as a function of the training set size

![plot of chunk unnamed-chunk-3](assets/fig/unnamed-chunk-3-1.png) 

--- .class #id 

## Summary

This plot is showing absolute difference Good and Bad probabilities. If it small them we can conclude that model not sure about whcih class should be for that image.
<br><br>
Additionally we can see which images was classified incorrectly as False Positives (FP) and False Negatives (FN)

![plot of chunk unnamed-chunk-4](assets/fig/unnamed-chunk-4-1.png) 



