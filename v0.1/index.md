---
layout: page
title: Tracks specification
---


## Definition

This is an example of track specification:

- Object: description
- Segment: description
- Track: description

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