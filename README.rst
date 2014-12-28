tz_select - Display an HTML select menu of time zones with Lasso
================================================================

Read the article `tz_select - Display an HTML select menu of time zones with Lasso
<http://www.stevepiercy.com/articles/tz_select-display-an-html-select-menu-of-time-zones-with-lasso/>`_.

Description
===========

``[tz_select]`` returns an HTML select menu of all known time zones, grouped
into US common, continents, regions, UTC, and manual offsets.

It is required by the demos for `tz_convert
<http://www.stevepiercy.com/lasso/tz_convert_demo/>`_ and `countdown
<http://www.stevepiercy.com/lasso/countdown_demo/>`_.

Demo
====

`Demo <http://www.stevepiercy.com/lasso/tz_select_demo/>`_.

Usage
=====

``tz_select`` requires one parameter and a second parameter is optional.

``-name`` is required and must be a string type. Its value must be the name of
the select HTML menu.

``-selected`` is optional but must be a string type. Its value should be the
value of the selected time zone.

Example
=======

.. code-block:: html+lasso

    <div>
    <label>Timezone From</label>
    [tz_select(-name='tzin', -selected=action_param('tzin'))]
    </div>

Output is a select HTML menu.

Installation and Requirements
=============================

The repository contains the tag ``[tz_select]`` in a file named
``tz_select.inc`` and a directory ``tz_select_demo`` containing the demo.
In this directory there is a web page named ``index.lasso`` containing the
``tz_select`` tag.

Install and configure the following requirements.

More Information
================

* `List of tz database time zones
  <http://en.wikipedia.org/wiki/List_of_tz_database_time_zones>`_
* `tz database, also called the zoneinfo database or IANA Time Zone Database
  <http://en.wikipedia.org/wiki/Tz_database>`_
