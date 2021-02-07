.. _release_proxy_clientbase:


VOKEN Proxy ClientBase
======================

You can start a VOKEN Proxy-ClientBase on your desktop or laptop PC now.
It would provide a standard local Socks5/HTTP proxy for you, which is based on vnTUNNEL (encrypted).


.. _proxy_clientbase_download:

Download
--------

VOKEN Proxy App for windows v0.9.28
   - `Download Portable Edition from Github.com <https://github.com/voken1000g/proxy_clientbase/releases/download/v0.9.28/voken-proxy-0.9.28.7z>`_
   - `Download Installer from Github.com <https://github.com/voken1000g/proxy_clientbase/releases/download/v0.9.28/voken-proxy-0.9.28.exe>`_

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
2. Extract the **voken-proxy-0.9.28.7z** to a new folder, or run **voken-proxy-0.9.28.exe** to install


Launch and initialize
---------------------

Just run the **VOKEN Proxy.exe**, and follow the prompts to initialize.

.. image:: /_static/proxy_clientbase/initialize0.png
   :width: 100 %
   :alt: initialize0.png
   :align: center


.. image:: /_static/proxy_clientbase/initialize1.png
   :width: 100 %
   :alt: initialize1.png
   :align: center


Proxies
-------

Select a proxy and connect

.. image:: /_static/proxy_clientbase/proxies.png
   :width: 100 %
   :alt: proxies.png
   :align: center


Click the **Proxies**, choose a ProxyContainer to connect.

.. Then a standard Socks5 proxy ``socks5://127.0.0.1:5678``,
and a HTTP proxy ``http://127.0.0.1:5679`` are ready for you.
And also, you can check your balance, or make transactions there.



Setting: System Proxy
---------------------

.. image:: /_static/proxy_clientbase/system_proxy.png
   :width: 100 %
   :alt: system_proxy.png
   :align: center

By setting the system proxy to `ON`,
most of your applications (include your browsers) could use the proxy automatically.




Settings: Proxy type
--------------------

.. image:: /_static/proxy_clientbase/only_pac.png
   :width: 100 %
   :alt: only_pac.png
   :align: center

The default proxy type is ``GLOBAL``,
if you want to enable the ``PAC Mode``,
just click ``Only PAC`` or ``Except PAC``.

PAC configuration file: ``./resources/app/backend/pac.xml``, for advanced, you can edit it manually.

