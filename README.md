AllJoyn Code Generator Tool Available! 
======================================

The AllJoyn team is excited to announce a new tool for developers - the
Code Generator.  If you have your AllJoyn service interface specification
defined, you can run the CodeGen tool and have it generate working sample
source code for both your service and client.  This tool, currently
supporting Linux (it may also work on and for Windows, but we haven't
validated it) and C++ bindings only, allows you the developer to get to the
domain-specifics, the real meat of your AllJoyn application more quickly,
by providing for you the "boilerplate" that all AllJoyn apps share.  This
includes the bus-attachment logic, object creation, interface binding, and
the marshalling/unmarshalling of messages that correspond to the various
methods and signals that comprise the service object.

The input to the Code Generator is an XML file which describes your service
object(s) and interface(s).  The output is a collection of C++ files for
the service and client, as well as makefiles necessary to build these two
entities.  Most of these output files are ready to be compiled.  Several
contain skeleton code that you will flesh out according to the needs of
your particular application.  This means you only need to implement the
methods, signals and properties specified by your interface(s), while the
Code Generator handles all of the AllJoyn 'plumbing'.

You can even have the Code Generator easily produce a fully runnable
service and client, invoking your AllJoyn methods and signals with default
data.  This immediately compilable/linkable/runnable system should be a
great help in learning and using the AllJoyn concepts in C++.

Because the Code Generator is being released as Open Source, you also have
the opportunity to extend and improve it.  It comes with its own
unit-testing framework and extensive collection of unit test input XML
files, which can also serve as examples XML interface definitions.

The AllJoyn code generator is available as source only, and is super easy
to build (we included a shell script to do so), and is available on GitHub
at the following URL: https://github.com/alljoyn/alljoyn_codegen

We hope this tool is a useful addition to your development environment.
Enjoy!

