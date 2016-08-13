# LIST PACKAGES BY INSTALL DATE
## Introduction
List "recent" packages homebrew has installed.

## Motivation
Installed a bunch of tools which had a bunch of dependencies. Used third-party taps. I have now finished with these tools and the dependencies and want to remove them, but I have no idea what their names were (and they are days ago in my bash history). What did I install that day? 

## Proposed solution
A new brew command, e.g. `brew list --date DDMMYY` or `brew list recent X` where X is the most recent X number of packages.

## Detailed design
If you run `brew info [package]` on an installed package, brew tells you the date it was poured. So this info is logged, we just need to search by this field.

## Alternatives considered
Can't think of any.
