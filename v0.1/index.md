---
layout: page
title: Specification
---


## Definition

This is an example of a track specification:

- **Object**: an object of interest (such a cell) detected in a microscopy image
- **Segment**: a linear, temporal collection of objects
- **Track**: a collection of segments

## Scenarios

### A simple track

The following shows an input consisting of 3 images.

The case illustrated shows 3 objects identified in each frame. At this stage, there is no associations between objects across the frames.

![1](images/SimpleTrack_objects.png){:class="img-responsive"}

The **objects table** is:

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

With a linking algorithm, an association is created between objects across frames, and segments are produced. The colored lines in the next figure represent these segments.

![2](images/SimpleTrack_links.png){:class="img-responsive"}

The **segments table** is:

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

In this table, the foreign key to the segments table is the **Object_ID**. This specification requires unique **Object_ID** in the objects table. If this is not the case, an extra **frame** column is necessary in the segments table.

Finally, tracks are derived from objects + segments information:
![3](images/SimpleTrack_tracks.png){:class="img-responsive"}

In this simple case, the tracks table would look like this:

Track_ID |  Segment_ID
---------|------------
 1       |    1
 2       |    2
 3       |    3

### Gap-closing

### Merge/split events

#### A merge event
#### A split event
