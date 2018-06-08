# Project Goals

## Self-driving car stack for StreetDrone on Nvidia PX2
OpenStreetDrone’s primary focus is to develop a fully functional, well-designed and high quality self-driving car software stack based on the Robot Operating System (ROS). The primary deployment platform is the Nvidia PX2 and the control interface is the Drive-By-Wire System defined and supplied by StreetDrone on the StreetDrone ONE.

## Open Source
OpenStreetDrone should remain freely usable for both open source and proprietary applications. To that end, we reuse the BSD 3-clause license inherited from the fork from Autoware. Specifically, we aim for licensing compatible with Apache 2.0 and we have no intention of moving to a more restrictive licence that would force users to open source their proprietary code. In addition, we strive to create a courteous, welcoming environment that feels approachable to newcomers. 

## Maintainability
ROS provides for a modular scalable architecture and there are already many high quality nodes maintained by the ROS open source community. OpenStreetDrone strives to reuse such nodes wherever possible to reduce the maintenance burden on project developers. Where changes are required to other open source nodes we seek to engage with the open source community to push changes upstream. We seek to base the code on long term support versions of ROS and Ubuntu.

## Stability
The main OpenStreetDrone code base should always maintain a high degree of stability. This means that crashes, hangs and regressions should be dealt with promptly, rather than letting them pile up.

## Quality
The main OpenStreetDrone code base should always maintain a high degree of code quality. We achieve this by maintaining a clear set of functional requirements and live design documents describing the architecture. For the implementation, quality is achieved by adhering to a common coding style, code reviews, continuous integration (automated build and regression tests), simulations and static analysis. We always build with ‘warnings as errors’ on by default. We recognise [AUTOSAR CPP14 guidelines](https://www.autosar.org/fileadmin/user_upload/standards/adaptive/17-10/AUTOSAR_RS_CPP14Guidelines.pdf) as a reference for good coding practice for C++ development and PEP8 for Python.  

## Simplicity
To make rapid progress possible, we try to keep the code relatively easy to understand, even though robotics and autonomous driving is complicated. We follow the design philosophy that each component (ROS node) should do one thing and do it well.  We try to use straightforward, well understood interfaces, algorithms and data structures when possible, we try to write clear, maintainable code, and we continue to improve names and code structure to aid understanding. When tricky “rocket science” code is truly needed to solve some problem, we try to keep it bottled up behind clean interfaces. In addition, we make heavy use of automated regression tests as a safety net, to allow aggressive changes with less risk of regressions.

## Performance
Performance is an important but secondary goal.  The software should be performant enough to run at sufficiently high frequencies on the Nvidia PX2 for normal operation.

## Security
Security is an important but secondary goal. We will seek to ensure that the software cannot be hacked or exploited by a third party.

# Out of scope
There are a few points which we consider out of scope for the project:

## OpenStreetDrone is an engineering project not a science project
For new features to be adopted into the project, we strongly prefer for the algorithms and technology to be mature or at least the use case for it to be proven.

## OpenStreetDrone is not a bundle of maximally general and reusable code
We build some general-purpose parts, but only to the degree needed to be a high quality self-driving car stack.

## OpenStreetDrone is not a general self-driving car stack
While the code might be ported to another hardware platform and control another different vehicle, that is for others to do and it is not a goal of the project to support such activities.
