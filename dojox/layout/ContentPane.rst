.. _dojox/layout/ContentPane:

========================
dojox.layout.ContentPane
========================

:Project owner: ?--
:since: V?

.. contents ::
   :depth: 2

dojox.layout.ContentPane is an extension to dijit.layout.ContentPane providing script execution, among other things.

Introduction
============

TODO: introduce the component/class/method


Usage
=====

TODO: how to use the component/class/method

.. js ::

   // your code



Examples
========

Programmatic example
--------------------

TODO: example

Declarative example
-------------------

TODO: example


See also
========

* `Executing JavaScript inside Content Panes <http://dojocampus.org/content/2008/07/30/executing-javascript-inside-content-panes/>`_
* through the use of the scriptHasHooks setting, a :ref:`Deferred instance <dojo/Deferred>`, onLoadDeferred and it's then() method, you can simulate the dojo.ready behavior from inside the loaded content.
* An alternative is to set scriptHasHooks=true, and have content like this in your loaded content:

.. js ::
 
   dojo.connect(_container_, "onLoad", function(){
      /* your script */
   });

This will connect your local function to the onLoad callback of the enclosing ContentPane.
