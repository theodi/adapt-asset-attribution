adapt-asset-attribution
=======================

A patch file for the adapt authoring tool that adds asset source, licence and attribution fields to the asset manager and automatically populates the attribution field in graphic components from this data.

# Requirements
This is testing on authoring tool version 0.10.3 but should also work on older versions. 

# Prep

Drop the patch file in the top level directory of the authoring tool

# Testing

> patch -p 1 --dry-run < patch.diff

If you get errors, maybe post an issue! 

# Deploying

> patch -p 1 < patch.diff

> grunt build:prod

Then restart your authoring tool.
