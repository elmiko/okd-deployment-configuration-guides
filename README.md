# OpenShift Deployment Configuration Notes

This repository contains a collection of documents describing known deployment configurations
for OpenShift. The information is categorized by deployment platform and installation options,
and tracks with the current release of the [OpenShift Container Platform](https://docs.openshift.com/container-platform/latest)
except where noted. Please note, these documents describe configurations for newly installed clusters
and do not include resources which may be required during installation (eg bootstrap instances).

These notes serve as a common place for sharing platform configurations, and exposing more of the
[tribal knowledge](https://en.wikipedia.org/wiki/Tribal_knowledge) that has been aquired by
developers and operators working closely with OpenShift.

## Repository structure

The files in this repository are divided into directories for each specific deployment platform.
Within each directory are [Markdown](https://www.markdownguide.org/) files for different deployment
scenarios. For example, most platforms will have a "Default IPI" document which describes the configuration
for a cluster that has been created using the [OpenShift installer](https://github.com/openshift/installer)
with a minimal configuration file.

## Contributing to the notes

Contributions to the notes are welcomed through pull requests from forked versions of this repository.

When proposing changes to the repository, place your content in the platform directory associated with your notes.
Within each directory, look for a file with a similar configuration to your changes. If none exists you
should create a new file that indicates what configuration you are describing. For example, if writing about
deploying in a disconnected network scenario, you might create a file named `IPI-disconnected-network.md`.

For inspiration about how to structure content within your document, please see one of the `IPI-default.md`
files.

And if all else fails, please do not hesitate to open your pull request and start a discussions with your
questions and concerns about implementation.
