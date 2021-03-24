# OKD Deployment Configuration Guides

This repository contains a collection of community curated documents describing known deployment configurations
for [OKD](https://okd.io). The information is categorized by deployment platform/style and installation options. At a minimum,
these guides describe the necessary infrastructure and configuration for an OKD deployment. Where possible,
the guides go into deeper detail about installation and deployment options and proceedures used by the authors.

These guides serve as a common place for sharing platform configurations, and exposing more of the
[tribal knowledge](https://en.wikipedia.org/wiki/Tribal_knowledge) that has been aquired by
developers and operators working closely with OKD.

## Repository structure

The files in this repository are divided into directories for each specific deployment platform or style.
Within each directory are [Markdown](https://www.markdownguide.org/) files for different deployment
scenarios. For example, most platforms will have a "Default IPI" document which describes the configuration
for a cluster that has been created using the [OpenShift installer](https://github.com/openshift/installer)
with a minimal configuration file.

## Contributing to the notes

Contributions to the notes are welcomed through pull requests from forked versions of this repository.

When proposing a new guide, please use the [Guide Template](guide-template.md) to create your content.
You should place your content in a platform directory associated with your specific deployment. You
should name your document using the installation method and brief descriptive text of the options
you are detailing. For example, if writing about deploying in a disconnected network scenario, you might
create a file named `UPI-disconnected-network.md`. If you are documenting your personal "home lab" setup,
please use your github username in the filename, for example `UPI-elmiko.md`.

And if all else fails, please do not hesitate to open your pull request and start a discussions with your
questions and concerns about implementation.
