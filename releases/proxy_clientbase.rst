.. _release_proxy_clientbase:


VOKEN Proxy ClientBase
======================

You can start a VOKEN Proxy-ClientBase on your desktop or laptop PC now.
It would provide a standard local Socks5/HTTP proxy for you, which is based on vnTUNNEL (encrypted).


.. _proxy_clientbase_download:

Download
--------

VOKEN Proxy Clientbase v0.9.14 (for Windows)
   - `Download from Github.com <https://github.com/voken1000g/proxy_clientbase/releases/download/v0.9.14/voken_proxy_clientbase_v0.9.14.7z>`_

If you do not have the Java JDK installed on your computer,
choose one of the following to download:

.. _java_jdk_download:

Java JDK 8 Update 271 (for Windows 64 bit), choose one below:
   - `Download from FileHorse <https://www.filehorse.com/download-java-development-kit-64/55825/download/>`_
   - `Download from Oracle.com <https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html>`_
   - `Download from Github.com <https://github.com/voken1000g/download/releases/download/public/jdk-8u271-windows-x64.exe>`_

Java JDK 8 Update 271 (for Windows 32 bit)
   - `Download from FileHorse <https://www.filehorse.com/download-java-development-kit-32/download/>`_
   - `Download from Oracle.com <https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html>`_
   - `Download from Github.com <https://github.com/voken1000g/download/releases/download/public/jdk-8u271-windows-i586.exe>`_


Install
-------

1. Make sure you have the **Java JDK** installed
2. Extract the **VOKEN Proxy Clientbase v0.9.14 (for Windows)** to a new folder


Launch and initialize
---------------------

Just run the **clientbase.exe**, and follow the prompts to set the VOKEN Private Key.

.. image:: /_static/proxy_clientbase/initialize.png
   :width: 100 %
   :alt: initialize.png
   :align: center


Dashboard
---------

Select a proxy and connect

.. image:: /_static/proxy_clientbase/dashboard.png
   :width: 100 %
   :alt: dashboard.png
   :align: center


Open the **Dashboard**, choose a ProxyContainer on the left to connect.

Then a standard Socks5 proxy ``socks5://127.0.0.1:5678``,
and a HTTP proxy ``http://127.0.0.1:5679`` are ready for you.

And also, you can check your balance, or make transactions there.


Settings: Proxy type
--------------------

.. image:: /_static/proxy_clientbase/only_pac.png
   :width: 100 %
   :alt: only_pac.png
   :align: center

The default proxy type is ``GLOBAL``,
if you want to enable the ``PAC Mode``,
just click ``Only PAC`` or ``Except PAC``.

PAC configuration file: ``./config/pac.xml``, for advanced, you can edit it manually.


Setting: System Proxy
---------------------

By setting the system proxy to `ON`,
most of your applications (include your browsers) could use the proxy automatically.

