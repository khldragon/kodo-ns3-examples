Before You Start
================

.. _before_you_start:

The project description, licensing, source code and how to compile
are available `here <https://github.com/steinwurf/kodo-ns3-examples>`_.
Please follow the instructions shown there to get the project running.
**Once you have built the project**, you can follow this tutorial.

Overview
--------

Currently the repository ``kodo-ns3-examples`` contains 3 basic examples
in its main path regarding how to use the library with ns-3, namely:

* ``wifi_broadcast``: This example consists on broadcasting packets
  with RLNC from a transmitter to N receivers with an IEEE 802.11b WiFi
  channel.
* ``wired_broadcast``: This example consists on broadcasting packets
  with RLNC from a transmitter to N receivers with the same erasure channel.
* ``encoder_recoder_decoder``: This example shows the gain of RLNC
  with recoding in a 2-hop line network consisting of an encoder, N recoders and
  a decoder with different erasure rates. Recoding can be set on or off and
  erasure rates modified by command-line parsing.

Automated Builds
----------------

You can check the build status of the repository master branch on our
`buildbot <http://buildbot.steinwurf.dk/stats?projects=kodo-ns3-examples>`_
page. Our buildbot display the supported combinations of platforms,
operating systems, and compilers. At the link, you can check
build status and build statistics for them in the respective waterfall link.
This information is provided also for other Steinwurf projects such as Kodo
itself.

What You Should Know Before the Tutorial
----------------------------------------

Kodo
^^^^

Kodo is a C++ library from `Steinwurf <http://www.steinwurf.com>`_ that
implements Random Linear Network Coding. The links you should review first to
get a clear idea of what the library does, are:

* `Kodo documentation <http://kodo.readthedocs.org/en/latest/>`_
* `Kodo source code <https://github.com/steinwurf/kodo>`_
* `Steinwurf buildbot <http://buildbot.steinwurf.dk/>`_

ns-3
^^^^

`ns-3 <http://www.nsnam.org/>`_ is a network simulator of the OSI layers
written in C++ for research and educational purposes under the GPLv2 license.
You can find documentation regarding a tutorial, a manual and a model
description in this `link <http://www.nsnam.org/documentation/>`_.

C++
^^^

In order for the tutorial to be easy to read, some basic knowledge of C++ is
recommended. If you are also a C++ beginner, you can refer to this
`tutorial <http://www.cplusplus.com/doc/tutorial/>`_ as a guide from the basics
to more advanced features of the language. Given that both ns-3 and Kodo are
highly based object oriented projects, we strongly recommend you to spend some
time on class related topics, particularly object properties (polymorphism,
inheritance) and templates (generic classes or functions based on abstract
types). In the mentioned C++ tutorial you may find plenty examples for this.

Waf
^^^

Our main building tool is ``waf`` in the same way it is for ns-3. So, if you
have used ns-3 before this should be transparent to you. If you have not used
``waf`` , you can review a description of the tool with some examples in the
`waf documentation <http://docs.waf.googlecode.com/git/apidocs_17/index.html>`_.
Nevertheless, we differ from ns-3's waf implementation and ``wscripts`` to fit
our particular needs. For this reason, we highly recommend you to follow the
instructions in the repository link mentioned at the beginning of this document.

Comments and Questions
----------------------

If for some reason your project does not build or you have any other issues or
questions related to the project, please feel free to contact us through our
`developers mailing list <http://groups.google.com/group/steinwurf-dev>`_.
Also, ns-3 users have their
`mailing list <https://groups.google.com/d/forum/ns-3-users>`_ so you can ask
questions strictly related to ns-3 there.
