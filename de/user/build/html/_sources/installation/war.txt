.. _installation_war:

Web-Archiv (WAR)
================

Der GeoServer ist als Standalone-Servlet zur Benutzung mit existierenden Servlet Container Anwendungen wie `Apache Tomcat <http://tomcat.apache.org/>`_ und `Jetty <https://jetty.mortbay.com/>`_ gepackt.

.. note:: GeoServer wurde am gründlichsten mit dem Tomcat getestet und aus diesem Grund könnten diese Instruktionen mit anderen Container-Anwendungen nicht funktionieren.

Java
----

GeoServer benötigt ein installiertes Java auf Ihrem System. Oracle Java SE 6 oder neuer wird dringend empfohlen. (Seit GeoServer 2.2.x wird Oracle JRE 5 nicht länger unterstützt.) Eine Java Development Kit (JDK) wird für die Ausführung vom Geoserver nicht benötigt. Für weitergehende Informationen über Java und GeoServer schauen Sie bitte in den Abschnitt :ref:`production_java`.

Installation
------------

#. Suchen Sie die `GeoServer Download Seite <http://geoserver.org/display/GEOS/Download>`_ auf und wählen Sie die geeignete Version zum Herunterladen aus.

#. Wählen Sie :guilabel:`Web-Archiv` auf der Download-Seite aus.

#. Laden Sie das Archiv herunter und entpacken es. Kopieren Sie die Datei :file:`geoserver.war` in das Verzeichnis, welches die Webapps Ihrer Container-Anwendung enthält.

#. Ihre Container-Anwendung sollte das Web-Archiv entpacken und automatisch den GeoServer aufsetzen und starten.

   .. note:: Der Neustart Ihrer Anwendung könnte notwendig sein.

Ausführung
----------

Verwenden Sie für Ihre Container-Anwendung vorgesehene Methode zum Starten und Stoppen von Webapps, um den GeoServer zu starten.

#. Öffnen Sie Ihren Browser und navigieren Sie zu  :file:`http://{container_application_URL}/geoserver`, um auf :ref:`web_admin` zuzugreifen. Mit einem auf Port 8080 laufenden Tomcat auf localhost würde die URL ``http://localhost:8080/geoserver`` lauten.

Deinstallation
--------------

#. Stoppen Sie die Container-Anwendung.

#. Entfernen Sie die GeoServer-Webapp aus dem Webapp-Verzeichnis Ihrer Container-Anwendung.
