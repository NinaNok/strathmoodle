moodle-availability_cohort
========================

[![Build Status](https://travis-ci.com/moodleuulm/moodle-availability_cohort.svg?branch=master)](https://travis-ci.com/moodleuulm/moodle-availability_cohort)

Moodle availability plugin which lets users restrict resources, activities and sections based on cohorts.


Requirements
------------

This plugin requires Moodle 3.7+


Motivation for this plugin
--------------------------

If your teachers want to restrict activities / resources / sections in their course to a subset of the course participants and these course participants share a common cohort, this plugin is for you.

Have a look at an example:

* The Moodle instance provides cohorts for each study subject and groups all students with the same subject in the corresponding cohort.
* Tim Teacher is an editing teacher in course A.
* If Tim wants to provide activities / resources / sections only for the students of a specific study subject, for example informatics, there is no possibility to achieve this with Moodle core functionality.

With availability_cohort, Tim can do this easily. He is just able to restrict his activities / resources / sections to a certain cohort and only the members of this cohort get access to the activities / resources / sections.


Installation
------------

Install the plugin like any other plugin to folder
/availability/condition/cohort

See http://docs.moodle.org/en/Installing_plugins for details on installing Moodle plugins


Usage & Settings
----------------

After installing the plugin, it is ready to use without the need for any configuration.

Teachers (and other users with editing rights) can add the "cohort" availability condition to activities / resources / sections in their courses. While adding the condition, they have to define the cohort in which students are a member in to access the activity / resource / section.

If you want to learn more about using availability plugins in Moodle, please see https://docs.moodle.org/en/Restrict_access.


How this plugin works / Pitfalls
--------------------------------

We created this availability plugin to ease the use case which is described above. The availability plugin just checks if the user is in the given cohort and, if yes, grants access to the restricted activity.


Theme support
-------------

This plugin is developed and tested on Moodle Core's Boost theme.
It should also work with Boost child themes, including Moodle Core's Classic theme. However, we can't support any other theme than Boost.


Plugin repositories
-------------------

This plugin is published and regularly updated in the Moodle plugins repository:
http://moodle.org/plugins/view/availability_cohort

The latest development version can be found on Github:
https://github.com/moodleuulm/moodle-availability_cohort


Bug and problem reports / Support requests
------------------------------------------

This plugin is carefully developed and thoroughly tested, but bugs and problems can always appear.

Please report bugs and problems on Github:
https://github.com/moodleuulm/moodle-availability_cohort/issues

We will do our best to solve your problems, but please note that due to limited resources we can't always provide per-case support.


Feature proposals
-----------------

Due to limited resources, the functionality of this plugin is primarily implemented for our own local needs and published as-is to the community. We are aware that members of the community will have other needs and would love to see them solved by this plugin.

Please issue feature proposals on Github:
https://github.com/moodleuulm/moodle-availability_cohort/issues

Please create pull requests on Github:
https://github.com/moodleuulm/moodle-availability_cohort/pulls

We are always interested to read about your feature proposals or even get a pull request from you, but please accept that we can handle your issues only as feature _proposals_ and not as feature _requests_.


Moodle release support
----------------------

Due to limited resources, this plugin is only maintained for the most recent major release of Moodle. However, previous versions of this plugin which work in legacy major releases of Moodle are still available as-is without any further updates in the Moodle Plugins repository.

There may be several weeks after a new major release of Moodle has been published until we can do a compatibility check and fix problems if necessary. If you encounter problems with a new major release of Moodle - or can confirm that this plugin still works with a new major relase - please let us know on Github.

If you are running a legacy version of Moodle, but want or need to run the latest version of this plugin, you can get the latest version of the plugin, remove the line starting with $plugin->requires from version.php and use this latest plugin version then on your legacy Moodle. However, please note that you will run this setup completely at your own risk. We can't support this approach in any way and there is a undeniable risk for erratic behavior.


Translating this plugin
-----------------------

This Moodle plugin is shipped with an english language pack only. All translations into other languages must be managed through AMOS (https://lang.moodle.org) by what they will become part of Moodle's official language pack.

As the plugin creator, we manage the translation into german for our own local needs on AMOS. Please contribute your translation into all other languages in AMOS where they will be reviewed by the official language pack maintainers for Moodle.


Right-to-left support
---------------------

This plugin has not been tested with Moodle's support for right-to-left (RTL) languages.
If you want to use this plugin with a RTL language and it doesn't work as-is, you are free to send us a pull request on Github with modifications.


PHP7 Support
------------

Since Moodle 3.4 core, PHP7 is mandatory. We are developing and testing this plugin for PHP7 only.


Copyright
---------

Ulm University
Communication and Information Centre (kiz)
Kathrin Osswald

The development of this plugin was started on the Moodle DACH conference in Zurich (2018). 
The other contributer we would like to give credits for:
Guido Hornig, <info@lernlink.de>

