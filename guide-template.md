---
authors:
  - "@elmiko"
last-updated: "2021-03-24"
okd-version: "X.Y"
---
# OKD Deployment Configuration Guide Template

```
<TODO: replace this block with your content>

Hello! This is the template for creating new OKD deployment configuration guides.
The text in this template provides instructions and suggestions to help you in
creating your guide, it is meant to be replaced as you write.

First steps:
* Update the header material. The section at the top of this document contains information about
  the document authors, the last date of update, and the target okd version for the guide. Please use
  your GitHub handle in the author section, and the date formatted as YYYY-MM-DD.
* Change the title. It is useful to specify what distinguishes your guide from others. For example
  "IPI AWS Deployment Using Cluster-Wide Proxy", or "Charro's Single Node LibVirt UPI Deployment".
* Follow the sections of this document and replace the content with your guide.
```

## Audience

```
<TODO: replace this block with your content>

Who is the primary intended audience for this guide? Is it the home hacker, or the engineer interested
in improving their cloud infrastructure, or someone else completely? This section should be used to highlight
what groups might get the most benefit from this guide.
```

## Prerequisites

Before beginning this guide, please review these prerequisites:

```
<TODO: replace this block with your content>

Use this section to talk about things that will be needed, or assumed available, for your deployment
configuration.

* Basic familiarity with Linux command line tools and installation process
* A network with a configurable router for your cluster
* USB thumb drive for boot media
* Access to a DNS server
```

## Infrastructure

The following hardware and services were used to construct this OKD cluster.

```
<TODO: replace this block with your content>

This section should describe the hardware configuration and topology you have used for your deployment.
Feel free to create sub-headings for special equipment or configurations you might have used, along
with descriptions of their usage.
```

### Compute

```
<TODO: replace this block with your content>

* Control plane nodes, 3 x AMD Ryzen 3 3300U, 64 GB RAM, 500 GB SSD
* Worker nodes, 2 x Intel Core i7-6800K, 128 GB RAM, 500 GB SSD
* Big worker node, 1 x AMD Ryzen 3990X, 1 TB RAM, 4 TB SSD
  * 1 x NVIDIA V100
  * Storage is 3 x 2 TB SSD in RAID configuration
```

### Networking

```
<TODO: replace this block with your content>

* Gigabit LAN between workstation, bootstrap, master node
* Gigabit LAN between master and worker nodes
* Gigabit LAN between master and router
* the LAN's and workstation's nameservice delegating requests of the wildcard domain to the master nodes
* 2 x GCP Load Balancers
```

## Deployment

```
<TODO: replace this block with your content>

This section is where you will describe your deployment and how you created and configured it. The
subsections here are given as inspiration for your content, feel free to remove or add where
appropriate.
```

### Setup

```
<TODO: replace this block with your content>

This section is for in-depth explanations of any setup work that was done before deployment.

* How did you prepare for your deployment?
* Did you create any extra services that a reader should know about?
* Describe the steps you took to prepare your infrastructure for deployment.
* Use `code blocks` to share relevant scripts and commands that your ran.
```

### Installation

```
<TODO: replace this block with your content>

This section is where you can talk about how you ran the installation process, and what options you chose along the way.

* How did you install your cluster?
* Are there any special considerations before attempting a similar process?
* Describe the steps you took to install OKD on your infrastructure.
* Use `code blocks` to share relevant scripts and commands that your ran.
```

### Upgrade

```
<TODO: replace this block with your content>

If you have performed upgrades on your deployment, this is the section to talk about how you did them.

* Are upgrade a part of your deployment?
* How do you plan and release them?
* Describe how you have performed upgrades and any extra steps you needed.
```

## Day 2 Operations

```
<TODO: replace this block with your content>

This section is for detailing things you have done with your cluster after the basic installation.

* After deployment what have you done to configure your cluster further?
* Are there other services or operators that you install?
* Is there additional automation that you use on cluster?
```

## Additional Resources

```
<TODO: replace this block with your content>

Use this section to add links to any materials that you referenced or would like to call out specifically.

You can also use this section to embed videos demonstrating your deployment and its configuration.
```

