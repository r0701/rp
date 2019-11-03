---
title: "Tracking In The Wild"
date: 2019-09-25T09:07:51+04:00
draft: true
---
# Tracking In The Wild Summary

## Trackers our team worked on

- [DSST](http://www.cvl.isy.liu.se/en/research/objrec/visualtracking/scalvistrack/index.html)
- [SRDCF](https://www.cvl.isy.liu.se/research/objrec/visualtracking/regvistrack/)

## DSST

### How it works

The DSST (Discriminative Scale Space Tracker) tries to solve the Robust scale estimation problem by learning discriminative correlation filters based on a scale pyramid representation. The author's results show that separating the filters for translation and scale estimation "improves the performance compared to an exaustive scale search"[1].

### Video result

**First video**: The tracker performed badly in the video where a couple where moving from the left to the right of the video frame. It lost the couple within the first few seconds and was not able to track them properly after that

**Second video**: The tracker performed much better in the sidewalk video and was able to track the person crossing the sidewalk. This may be due to better lighting and less occlusion variations.

## SRCDF

### How it works

Regularized Discriminative Correlation Filters (SRDCF) focuses on mitigating the "unwanted boundry effects, which limits the performance of standard correlation based trackers"[2].

### Video result

**First video**: The tracker outperformed the DSST tracker on the same first video (Couples). The tracker does a good job following the couple as they move from the left to the right of the video frame.

**Second video**: The tracker was able to keep on target from the initial frame to the final frame without any issues when tracking the person crossing the crosswalk.

## Conclusion

Only using the two videos as benchmark, it is obvious that the SRCDF outperforms the DSST tracker. A reason could be that the SRCDF has a better occlusion performance than the DSST. Another reason may be that the SRCDF has a better performace when lighting varies in the sample video. 

## Bibliography

```
1. Danelljan, Martin, et al. "Discriminative scale space tracking." IEEE transactions on pattern analysis and machine intelligence 39.8 (2016): 1561-1575.
2. Danelljan, Martin, et al. "Learning spatially regularized correlation filters for visual tracking." Proceedings of the IEEE international conference on computer vision. 2015.
```
