
#### Multitenancy:

**What is it?**

Multitenancy refers to the hosting of multiple isolated virtual machines on a single piece of hardware, hence there being 'multiple tenants', this piece of hardware (a server) can be upgraded as and when required, this is an example of vertical scaling.

**Why is it important?**

This is important as it is a core feature of Amazon EC2, it allows for VMs to be started, upgraded, and terminated as and when required. Users only pay for active VMs.

#### Instance types:

- General Purpose: For general purpose tasks with no prioritisation of resources.
- Compute Optimised: For compute heavy tasks.
- Memory Optimised: For memory heavy tasks.
- Storage Optimised: For storage heavy tasks.
- Accelerated Computing: For graphics and data-matching tasks.

#### Machine image

An AMI or Amazon Machine Images are templates that can be loaded into an EC2 instance, these dictate the operating system, memory, storage, and software that will be loaded on deployment.

Example: Ubuntu, 128GB RAM, 8TB Storage.

EC2 follows the same pay as demand / pay on usage model as the rest of AWS.

#### Further instance types:

- Dedicated Instance: an instance that can be privately reserved for a business.
- Spot Instance: these are cheaper instances that AWS can reclaim on short notice.

Each instance has it's own pros and cons, so they should be chosen with caution.

#### Scaling EC2:

EC2 can be scaled using a mechanic called elasticity, this means that EC2 instances can automatically grow and shrink in response to real time usage, this is extremely effective in ensuring consistent uptime. This can involve either increasing the resources on one instance (vertical scaling), or creating more EC2 instances (horizontal scaling).

