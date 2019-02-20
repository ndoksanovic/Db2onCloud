---

copyright:
  years: 2014, 2019
lastupdated: "2019-01-02"

---

<!-- Attribute definitions --> 
{:javascript: #javascript .ph data-hd-programlang='javascript'}
{:java: #java .ph data-hd-programlang='java'}
{:ruby: #ruby .ph data-hd-programlang='ruby'}
{:php: #php .ph data-hd-programlang='php'}
{:python: #python .ph data-hd-programlang='python'}
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:important: .important}
{:note: .note}
{:deprecated: .deprecated}
{:pre: .pre}

# Einführung
{: #getting_started_db2oncloud}

Bei {{site.data.keyword.Db2_on_Cloud_long}} handelt es sich um eine SQL-Datenbank, die für Sie in der Cloud bereitgestellt wird. Sie können {{site.data.keyword.Db2_on_Cloud_short}} wie jede andere Datenbanksoftware verwenden, der Aufwand und die Kosten für die Hardwareeinrichtung sowie die Softwareinstallation und -verwaltung fallen jedoch weg. 
{: shortdesc}

Erstellen Sie Berechtigungsnachweise. Für neue Benutzer von IBM Cloud: Nach der Erstellung des Service müssen Sie einen Benutzernamen und ein Kennwort erstellen, indem Sie beim Starten des Service auf die Schaltfläche **Berechtigungsnachweise erstellen** klicken. Es ist technisch möglich, sich bei der Webkonsole ohne Berechtigungsnachweise anzumelden, Sie benötigen jedoch den Benutzernamen und das Kennwort zur Verwendung zahlreicher Db2-Tools.
{: important}

Es ist ebenfalls möglich, eine lokale Db2-Datenbank mithilfe des [kostenfreien Downloads für Db2 Developer Edition ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://www.ibm.com/us-en/marketplace/ibm-db2-direct-and-developer-editions){:new_window} zu installieren. Dabei wird ohne großen Zeitaufwand eine sofort einsatzfähige Db2 Developer Edition-Instanz mit Tools in einem Docker-Container installiert (Docker nicht erforderlich; alle erforderlichen Komponenten werden automatisch installiert). 

<!-- ## Free trial
{: #freetrial}

You can try the {{site.data.keyword.Db2_on_Cloud_short}} Precise Performance 500 (2.8.500) plan for 7 days on {{site.data.keyword.Bluemix_notm}} without charge. [Free trial ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://console.bluemix.net/catalog/services/db2){:new_window} -->

## Schnittstellen
{: #interfaces}

Für die Arbeit mit der {{site.data.keyword.Db2_on_Cloud_short}}-Datenbank stehen Ihnen die folgenden Möglichkeiten zur Verfügung:
{: shortdesc}

   * {{site.data.keyword.Db2_on_Cloud_short}}-Webkonsole
   * REST-API
   * Herstellen einer Verbindung für Anwendungen oder bevorzugte Tools vom lokalen Computer
   * Verwenden von {{site.data.keyword.Db2_on_Cloud_short}} als Datenquelle für {{site.data.keyword.Bluemix_notm}}-Apps oder -Services

### Db2 on Cloud-Webkonsole
{: #web_console}

Die Webkonsole bietet eine grafische Schnittstelle für alle Funktionen, die Sie für die Verwendung der Datenbank benötigen. Hierzu gehören z. B. Ladefunktionen, ein SQL-Editor, Treiberdownloads usw.
{: shortdesc}

<!-- ![View of Db2 on Cloud web console dashboard page](images/console_v2.png) -->
<!-- ![View of {{site.data.keyword.dashdbshort_notm}} web console dashboard page](images/console_v2.jpg) -->

<!-- Click the link to take a tour of the Db2 web console: [General tour ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://ibm.biz/dashdb-general-quick-tour){:new_window}. -->

Für den Zugriff auf die {{site.data.keyword.Db2_on_Cloud_short}}-Webkonsole stehen Ihnen die folgenden Möglichkeiten zur Verfügung:
   * Über das {{site.data.keyword.Bluemix_notm}}-Dashboard - Sie können die Webkonsole über die Servicedetailseite für Ihren {{site.data.keyword.Db2_on_Cloud_long_notm}}-Service öffnen.
   * Direkt über die URL - Sie können die URL der Webkonsole für Ihren {{site.data.keyword.Db2_on_Cloud_short}}-Service mit einem Lesezeichen markieren.

<!-- ###REST APIs
{: #apis}

With Db2 Warehouse plans, you can perform tasks related to file management, loading data, and running R scripts by using the [Db2 Warehouse REST API ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://ibm.biz/dashdb-api){:new_window}.
{: shortdesc} -->

### Db2-Befehlszeilenclients und -treiber auf dem Computer installieren
{: #connect_apps}

Die meisten Benutzer können diesen Schritt überspringen. In den meisten Fällen verwenden Benutzer bevorzugt die REST-API oder installieren Treiber für ein Framework, z. B. mit dem Python-Befehl `pip`. Professionelle Anwender können jedoch den Db2-Befehlszeilenclient verwenden, um Datenbanken zu verwalten und Db2-Befehle auszuführen. Darüber hinaus kann die Installation von Db2-Treibern grundsätzlich für bestimmte ODBC- oder JDBC-Anwendungen von Vorteil sein. Führen Sie in diesem Fall die folgenden Schritte aus:
{: shortdesc}

<!-- Drivers on site are broken so taking out this one -Simon. 1. Download the [driver package ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/support/knowledgecenter/SS6NHC/com.ibm.swg.im.dashdb.doc/connecting/connect_driver_package.html){:new_window} from the Connection info page of the {{site.data.keyword.Db2_on_Cloud_short}} web console.-->

1. [Installieren Sie das Treiberpaket ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://www.ibm.com/support/knowledgecenter/SS6NHC/com.ibm.swg.im.dashdb.doc/connecting/connect_driver_package_install.html){:new_window} auf dem Computer, auf dem Ihre Apps bzw. Tools ausgeführt werden.
2. [Konfigurieren Sie die Treiberdateien ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://www.ibm.com/support/knowledgecenter/en/SS6NHC/com.ibm.swg.im.dashdb.doc/connecting/connect_driver_package_config.html){:new_window} für Ihre {{site.data.keyword.Db2_on_Cloud_short}}-Datenbank.

### Verwenden von Db2 on Cloud als Datenquelle für {{site.data.keyword.Bluemix_notm}}-Apps oder -Services
{: #data_src}

Für Apps, die per Hosting in {{site.data.keyword.Bluemix_notm}} bereitgestellt werden, können Verbindungen zu Ihrer {{site.data.keyword.Db2_on_Cloud_short}}-Datenbank auf dieselbe Weise hergestellt werden wie bei Verbindungen für lokalen Anwendungen zu Ihrer {{site.data.keyword.Db2_on_Cloud_short}}-Datenbank.
{: shortdesc}

Wenn Ihre Apps die {{site.data.keyword.Bluemix_notm}}-Plattform verwenden, können Sie die Umgebungsvariable `VCAP _SERVICES` nutzen, um das Angeben von Datenbankdetails und -berechtigungsnachweisen zu vereinfachen:
1. Klicken Sie im {{site.data.keyword.Bluemix_notm}}-Dashboard auf der Registerkarte **Verbindungen** der Servicedetailseite für Ihren {{site.data.keyword.Db2_on_Cloud_long_notm}}-Service auf die Schaltfläche **Verbindung erstellen**.
2. Wählen Sie die {{site.data.keyword.Bluemix_notm}}-App aus, die mit der {{site.data.keyword.Db2_on_Cloud_short}}-Datenbank als Datenquelle verwendet werden soll, und klicken Sie dann auf die Schaltfläche **Verbinden**.
3. Aktualisieren Sie den Anwendungscode, um Datenbankdetails- und -berechtigungsnachweise aus der Umgebungsvariablen `VCAP_SERVICES` abzurufen.

    **Beispiel ohne `VCAP_SERVICES`**

    ```php
    <?php
    $driver      = "DRIVER={IBM DB2 ODBC DRIVER};";

    $database    = "BLUDB";         # Datenbankdetails von der
    $hostname    = "<Host-name>";   # Verbindungsseite der
    $port        = 50000;           # Db2 on Cloud-Webkonsole abrufen.
    $user        = "<Benutzer-ID >";    #
    $password    = "<Kennwort>";    #
    $dsn         = "DATABASE=$database;" .
                   "HOSTNAME=$hostname;" .
                   "PORT=$port;" .
                   "PROTOCOL=TCPIP;" .
                   "UID=$user;" .
                   "PWD=$password;";

    $conn_string = $driver . $dsn;

    $conn        = db2_connect( $conn_string, "", "" );
    ?>
    ```

    **Beispiel mit `VCAP_SERVICES`**

    ```php
    <?php
    $driver      = "DRIVER={IBM DB2 ODBC DRIVER};";

    $vcap        = json_decode( getenv( "VCAP_SERVICES" ), true );
    $dsn         = $vcap[ "dashDB" ][0][ "credentials" ][ "dsn" ];

    $conn_string = $driver . $dsn;
                                   
    $conn        = db2_connect( $conn_string, "", "" );
    ?>
    ```

## Beispiele
{: #samples}

Über die folgenden Links können Sie Beispiele aufrufen, die veranschaulichen, wie Sie eine Verbindung von Anwendungen in verschiedenen Sprachen zu Ihrer {{site.data.keyword.Db2_on_Cloud_short}}-Datenbank herstellen:
{: shortdesc}

   * [.NET ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://www.ibm.com/support/knowledgecenter/SS6NHC/com.ibm.swg.im.dashdb.doc/connecting/connect_connecting__net_applications.html){:new_window}
<!-- * [JAVA ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/support/knowledgecenter/SS6NHC/com.ibm.swg.im.dashdb.doc/connecting/connect_connecting_java.html){:new_window} -->
   * [JDBC ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://www.ibm.com/support/knowledgecenter/SS6NHC/com.ibm.swg.im.dashdb.doc/connecting/connect_connecting_jdbc_applications.html){:new_window}
<!-- * [Node.js ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/support/knowledgecenter/SS6NHC/com.ibm.swg.im.dashdb.doc/connecting/connect_connecting_nodejs.html){:new_window} -->
   * [PHP ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://www.ibm.com/support/knowledgecenter/SS6NHC/com.ibm.swg.im.dashdb.doc/connecting/connect_connecting_php.html){:new_window}
<!-- * [Python ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/support/knowledgecenter/SS6NHC/com.ibm.swg.im.dashdb.doc/connecting/connect_connecting_python.html){:new_window} -->
<!-- * [{{site.data.keyword.Db2_on_Cloud_short}} samples on GitHub ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://github.com/IBM-Bluemix/dashdb-nodejs-helloworld){:new_window} -->

## Video: Db2 on Cloud - Einführung
{: #intro_vid}

Dieses Video enthält eine Einführung in {{site.data.keyword.Db2_on_Cloud_short}}.

<iframe class="embed-responsive-item" id="youtubeplayer1" title="Einführung in {{site.data.keyword.Db2_on_Cloud_short}}" type="text/html" width="640" height="390" src="//www.youtube.com/embed/F_ylk44_WOg?rel=0" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen> </iframe>

## Video: Über die REST-API mit Db2 on Cloud kommunizieren
{: #vid_api}

Dieses Video veranschaulicht die Schritte, die erforderlich sind, um mithilfe einer REST-konformen API mit {{site.data.keyword.Db2_on_Cloud_short}} zu kommunizieren.

<iframe class="embed-responsive-item" id="youtubeplayer2" title="Kommunikation mit {{site.data.keyword.Db2_on_Cloud_short}} über eine REST-konforme API" type="text/html" width="640" height="390" src="//www.youtube.com/embed/PSNBDwgf9ts?rel=0" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen> </iframe>

## Video: Integration mit Jupyter-Notizbüchern
{: #cognos_vid}

Dieses Video veranschaulicht die Integration von Jupyter-Notizbüchern mit {{site.data.keyword.Db2_on_Cloud_short}}.

<iframe class="embed-responsive-item" id="youtubeplayer3" title="Integration von Jupyter-Notizbüchern" type="text/html" width="640" height="390" src="//www.youtube.com/embed/bNfH0Wzx3is?rel=0" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen> </iframe>

