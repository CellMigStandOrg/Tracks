---
layout: page
title: Specification
---


## Definition

This is an example of track specification:

- Object: description of an object
- Segment: a linear collection of objects
- Track: a collection of segments

## Scenarios

### Simple track

![A simple track](SimpleTrack.png){:class="img-responsive"}



Object_ID  |  Frame  |  X |  Y
-----------|---------|----|-----
1          |    1    |    |  
2          |    1    |    |  
3          |    1    |    | 
4          |    2    |    |
5          |    2    |    |
6          |    2    |    |
7          |    3    |    |
8          |    3    |    |
9          |    3    |    |


Segment_ID |  Object_ID
-----------|------------
 1         |    1
 1         |    4
 1         |    7
 2         |    2
 2         |    5
 2         |    8
 3         |    3
 3         |    6
 3         |    9


### Gap closing


### Merge/split events