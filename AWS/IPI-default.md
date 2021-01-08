# AWS IPI Default Deployment

This describes the resources used by OpenShift after perfoming an installation
using the default options for the installer.

## Compute

* 3 control plane nodes
  * instance type `m4.xlarge`, or `m5.xlarge` if previous not available in the region
* 3 compute nodes
  * instance type `m4.large`, or `m5.large` if previous not available in the region

## Networking

* 1 virtual private cloud
* 1 public subnet per availability zone in the region
* 1 private subnet per availability zone in the region
* 1 NAT gateway per availability zone
* 1 elastic IP address per NAT gateway
* 3 elastic load balancers
  * 1 external network load balancer for the master API server
  * 1 internal network load balancer for the master API server
  * 1 classic load balancer for the router
* 21 elastic network interfaces, plus 1 interface per availability zone
* 1 virtual private cloud gateway

## Security

* 10 distinct security groups