segment_displays:
=================

*Config file section*

+----------------------------------------------------------------------------+---------+
| Valid in :doc:`machine config files </config/instructions/machine_config>` | **YES** |
+----------------------------------------------------------------------------+---------+
| Valid in :doc:`mode config files </config/instructions/mode_config>`       | **NO**  |
+----------------------------------------------------------------------------+---------+

.. overview

The ``segment_displays:`` section of your config is where you define your
:doc:`segment displays </displays/display/alpha_numeric>`.
This can be 7-segment or alphanumeric displays which are typically
used in older machines.

.. config


Required settings
-----------------

The following sections are required in the ``segment_displays:`` section of your config:

number:
~~~~~~~
Single value, type: ``string``.

The number of the display. The meaning depends on the hardware platform.


Optional settings
-----------------

The following sections are optional in the ``segment_displays:`` section of your config. (If you don't include them, the default will be used).

platform:
~~~~~~~~~
Single value, type: ``string``.

This can be used to overwrite the platform which is defined in the *hardware*
section for segment_displays.

platform_settings:
~~~~~~~~~~~~~~~~~~
Single value, type: dict.

.. todo:: :doc:`/about/help_us_to_write_it`

console_log:
~~~~~~~~~~~~
Single value, type: one of the following options: none, basic, full. Default: ``basic``

Log level for the console log for this device.

debug:
~~~~~~
Single value, type: ``boolean`` (Yes/No or True/False). Default: ``False``

Set this to true to see additional debug output. This might impact the performance of MPF.

file_log:
~~~~~~~~~
Single value, type: one of the following options: none, basic, full. Default: ``basic``

Log level for the file log for this device.

label:
~~~~~~
Single value, type: ``string``. Default: ``%``

Name of this device in service mode.

tags:
~~~~~
List of one (or more) values, each is a type: ``string``.

Not used.


Related How To guides
---------------------

* :doc:`/displays/display/alpha_numeric`
* :doc:`/hardware/segment_display_platforms`
