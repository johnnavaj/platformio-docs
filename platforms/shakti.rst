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

.. _platform_shakti:

Shakti
======

:Configuration:
  :ref:`projectconf_env_platform` = ``shakti``

Platform SHAKTI is an open-source initiative by the RISE group at IIT-Madras, which is not only building open source, production grade processors, but also associated components like interconnect fabrics, verification tools, storage controllers, peripheral IPs and SOC tools.

For more detailed information please visit `vendor site <https://sifive.com?utm_source=platformio&utm_medium=docs>`_.

.. contents:: Contents
    :local:
    :depth: 1


Examples
--------

Examples are listed from `Shakti development platform repository <https://github.com/platformio/platform-shakti/tree/develop/examples>`_:

* `shakti-sdk_uart-hello <https://github.com/platformio/platform-shakti/tree/develop/examples/shakti-sdk_uart-hello>`_
* `shakti-sdk_gpio-keypad <https://github.com/platformio/platform-shakti/tree/develop/examples/shakti-sdk_gpio-keypad>`_
* `shakti-sdk_i2c-lm75 <https://github.com/platformio/platform-shakti/tree/develop/examples/shakti-sdk_i2c-lm75>`_

Debugging
---------

:ref:`piodebug` - "1-click" solution for debugging with a zero configuration.

.. contents::
    :local:


Tools & Debug Probes
~~~~~~~~~~~~~~~~~~~~

Supported debugging tools are listed in "Debug" column. For more detailed
information, please scroll table by horizontal.
You can switch between debugging :ref:`debugging_tools` using
:ref:`projectconf_debug_tool` option in :ref:`projectconf`.

.. warning::
    You will need to install debug tool drivers depending on your system.
    Please click on compatible debug tool below for the further instructions.

On-Board Debug Tools
^^^^^^^^^^^^^^^^^^^^

Boards listed below have on-board debug probe and **ARE READY** for debugging!
You do not need to use/buy external debug probe.

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

Stable and upstream versions
----------------------------

You can switch between `stable releases <https://github.com/platformio/platform-shakti/releases>`__
of SiFive development platform and the latest upstream version using
:ref:`projectconf_env_platform` option in :ref:`projectconf` as described below.

Stable
~~~~~~

.. code-block:: ini

    ; Latest stable version
    [env:latest_stable]
    platform = shakti
    board = ...

Upstream
~~~~~~~~

.. code-block:: ini

    [env:upstream_develop]
    platform = https://github.com/platformio/platform-shakti.git
    board = ...


Packages
--------

.. list-table::
    :header-rows:  1

    * - Name
      - Description

    * - `framework-shakti-sdk <https://gitlab.com/shaktiproject/software/shakti-sdk>`__
      - Open Source Software for Developing on the Shakti Platform

    * - `tool-jlink <https://www.segger.com/downloads/jlink/?utm_source=platformio&utm_medium=docs>`__
      - SEGGER J-Link Software and Documentation Pack

    * - `tool-openocd-riscv <https://github.com/riscv/riscv-openocd?utm_source=platformio&utm_medium=docs>`__
      - OpenOCD for RISC-V

    * - `tool-qemu-riscv <https://www.qemu.org/?utm_source=platformio&utm_medium=docs>`__
      - Open source machine emulator and virtualizer

    * - `toolchain-riscv <https://github.com/riscv/riscv-gnu-toolchain?utm_source=platformio&utm_medium=docs>`__
      - GNU toolchain for RISC-V, including GCC

.. warning::
    **Linux Users**:

        * Install "udev" rules :ref:`faq_udev_rules`
      
    **Windows Users:**

        Please check that you have a correctly installed USB driver from board
        manufacturer

Frameworks
----------
.. list-table::
    :header-rows:  1

    * - Name
      - Description

    * - :ref:`framework_shakti-sdk`
      - Open Source Software for Developing on the SiFive Freedom E Platform

Boards
------

.. note::
    * You can list pre-configured boards by :ref:`cmd_boards` command or
      `PlatformIO Boards Explorer <https://platformio.org/boards>`_
    * For more detailed ``board`` information please scroll tables below by
      horizontal.

Shakti
~~~~~~

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


