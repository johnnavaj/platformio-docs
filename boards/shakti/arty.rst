..  Copyright (c) 2014-present PlatformIO <contact@platformio.org>
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
       http://www.apache.org/licenses/LICENSE-2.0
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

.. _board_sifive_e310-arty:

Arty FPGA Dev Kit
=================

.. contents::

Hardware
--------

Platform :ref:`platform_sifive`: SiFive brings the power of open source and software automation to the semiconductor industry, making it possible to develop new hardware faster and more affordably than ever before. 


.. list-table::
    :header-rows:  1

    * - Name
      - Platform
      - MCU
      - Frequency
      - Flash
      - RAM
    * - :ref:`board_artix7_35t`
      - :ref:`platform_shakti`
      - E-Class
      - 50MHz
      - 0KB
      - 128KB
    * - :ref:`board_artix7_100t`
      - :ref:`platform_shakti`
      - C-Class
      - 50MHz
      - 0KB
      - 128MB

Configuration
-------------

Please use ``artix7_35t & artix7_100t`` ID for :ref:`board_artix7_35t` & :ref:`board_artix7_100t`:

.. code-block:: ini

  [env:artix7_35t]
  platform = Shakti
  board = artix7_35t
  
  [env:artix7_100t]
  platform = Shakti
  board = artix7_100t
  
Uploading
---------
Arty FPGA Dev Kit supports the next uploading protocols:

* ``ftdi``
* ``jlink``


Default protocol is ``ftdi``

Debugging
---------

:ref:`piodebug` - "1-click" solution for debugging with a zero configuration.

.. warning::
    You will need to install debug tool drivers depending on your system.
    Please click on compatible debug tool below for the further
    instructions and configuration information.

You can switch between debugging :ref:`debugging_tools` using
:ref:`projectconf_debug_tool` option in :ref:`projectconf`.

Arty FPGA Dev Kit has on-board debug probe and **IS READY** for debugging. You don't need to use/buy external debug probe.

.. list-table::
  :header-rows:  1

  * - Compatible Tools
    - On-board
    - Default
  * - :ref:`debugging_tool_ftdi`
    - Yes
    - Yes
  * - :ref:`debugging_tool_jlink`
    - Yes
    - Yes


Frameworks
----------
.. list-table::
    :header-rows:  1

    * - Name
      - Description

    * - :ref:`framework_shakti_sdk`
      - Open Source Software for Developing on the SiFive Freedom E Platform
