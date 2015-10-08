==========================================================
Widget system implementation for Horizon Overview web page
==========================================================

Summary
=======
This blueprint propose to change the Overview web page in order to be configurable using a Widget based-panel.

Motivation
==========
Until Juno release, the Overview web page offers information about the quotas, a filter for check the usage during a period of time and the list of first instances created. OpenStack offers much more information than that, like volumes and the quota volume, images, networking, orchestration, etc. and this information is not provide anyway right now in the Overview web page.
The idea of an Overview page could be get the more relevant information about the cloud in just one hit. Of course, "relevant information" depends on the user, each user wants to manage different data in the Overview page depending of its needs.
In this blueprint is decribed an alternative Overview web page to be able to configure it and get the most important information for the user.

Description
===========
The proposal in this paper is create a new Overview web page that can be configured, via Widgets, with the relevant information for the user.
A Widget is a HTML box with information, from some OpenStack API, shown in a certain way. For example, we can design a Widget to get information from Stacks or their resources. Other example, a Widget that shows who (user or group) is able to access into the current project. The widgets should be an isolated piece of code that can be plug and unplug to Overview page.
The capability to plug and unplug widget to Overview page could be allowed following the user organization that OpenStack has (roles, groups, users).
This new Overview page should optional via settings parameter.


UX
==


Wireframes, Mocks, Videos and UI Markup
---------------------------------------
None

Testing
=======
Unit tests should be provided per widget.

Outside Dependencies
====================
None

Requirements Update Required
============================
None

Doc Impact
==========
New sections in order to explain how to develop a Widget and how to manage them.
