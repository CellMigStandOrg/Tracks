---
layout: page
title: About
---

### Introduction

This document contains the working draft of the Tracks specification being
developed by the
[Cell Migration Standardisation Organisation (CMSO)](https://cmso.science/).

The current specification is based on *tracking by detection* techniques (see computational workflow in the following figure) and the data produced therein:

![workflow](images/workflow.png){:class="img-responsive"}

1.  A **segmentation algorithm** detects objects of interest (i.e. cells) in a
    set of microscopy images (usually time-lapse), producing *objects*
2.  A **linking algorithm** finds associations between these objects and links
    them in time, producing *links*
3.  A **segment linking** processes the links, identifying possible events
    (gap-closing, split, merge), producing final *tracks*

This specification aims at representing these data in a **tabular format**:

Data is held in a *table*. The properties of a table are:

- columns — the list of columns in the table
- rows — the list of rows in the table

For a formal specification of Tabular Data Models see
[Model for Tabular Data and Metadata on the Web-W3C](https://www.w3.org/TR/2015/WD-tabular-data-model-20150108/#model).

### Goals
The goal of this specification is to define a common, standard format to
represent cell tracking data associated with cell migration experiments.
The specification should:

- be simple and extensible
- re-use existing standard formats, where possible
- be associated with human- and machine-readable metadata

### Language
The key words `MUST`, `MUST NOT`, `REQUIRED`, `SHALL`, `SHALL NOT`, `SHOULD`,
`SHOULD NOT`, `RECOMMENDED`, `MAY`, and `OPTIONAL` in this specification are
to be interpreted as described in
[RCF 2119](https://www.ietf.org/rfc/rfc2119.txt).

### Links

See the [version 0.1](v0.1/index.md) of this specification.
