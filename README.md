# kalendarium

## Introduction

kalendarium is a LaTeX3 package that provides several macros with which to print dates in classical Latin given days on the Julian or Gregorian calendars, using the same syntax used by ancient Roman authors.  The format of these dates may be customised either in the package options or on a per-command basis; these options also allow for the generation of date strings according to different eras of the Classical period.

## Usage

Most simply, kalendarium may be imported with default formatting in the usual fashion, with the line `\usepackage{kalendarium}`.  Global formatting options may be set on import with key-value pairs as specified in the package documentation; for example, to display all dates in a document with no abbreviation, numbers fully written out in Latin, and years calculated *ab urbe condita*, this import string may be used:

```
\usepackage[abbreviate=false,dayfmt=latin,era=auc]{kalendarium}
```

If the command `\KalDate{1917}{11}{7}` is called with these options, the following date would be rendered: *ante diem septimum Idus Novembres MMDCLXX ab urbe condita*.

Formatting options may be set for individual macro invocations as well: all commands take an optional parameter that accepts the same keys as the import string.  More information on the formatting features provided by this package may be found in the package documentation.
