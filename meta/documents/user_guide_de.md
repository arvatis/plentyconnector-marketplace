# PlentyConnector plugin Shopware

## Produktinformationen

Der plentymarkets Shopware Connector (PSC7) wird von dem Expert Partner arvatis media entwickelt. Der Connector bietet eine Vielzahl erweiterter Möglichkeiten für einen besseren und schnelleren Abgleich - als Basis dient die moderne REST-API.

Nutzen Sie jetzt alle Vorteile von plentymarkets und der aktuellsten Shopware Version für die optimale eCommerce-Synergie aus Warenwirtschaft und individualisiertem Shop.

### Neuen Funktionen / neue Abgleiche des Connectors

Die neuste Version ist momentan nur über arvatis.com zu erwerben.

Für eine detaillierte Auflistung möchten wir gerne auf das ausführliche[ ](https://docs.google.com/document/d/10mPeV3xqx4We71dYQdPmJK2qvb21Rpym6FG_tKwHKfc/)<span class="c9">[Handbuch vom PSC7](https://docs.google.com/document/d/10mPeV3xqx4We71dYQdPmJK2qvb21Rpym6FG_tKwHKfc/edit?usp%3Dsharing&sa=D&ust=1507645556706000&usg=AFQjCNEVv48pBAe8ezFN7q5-XRZZma-FXA) verweisen.

Die arvatis media wird als betreuende Agentur freut sich jederzeit über konstruktive Kritik und weitere Anregungen zur fortlaufenden Optimierung.

Darüber hinaus erlaubt die modulare Opensource Gestaltung des neuen Connectors ebenfalls die individuelle Weiterentwicklung des Connectors oder die Bereitstellung neuer Funktionen.

## Installationsanleitung

Für die Einrichtung Ihrer plentymarkets 7 und Shopware-Anbindung sind einige wichtige Voraussetzungen zwingend erforderlich, um eine dauerhaft reibungslose Synchronisation der Daten beider Systeme zu gewährleisten,

### Systemvoraussetzungen

*   plentymarkets
*   mindestens Shopware-Version 5.7.0
*   Ein für Shopware eingerichteter Mandant in plentymarkets
*   <span class="c11">In Shopware sind alle benötigten Kundengruppen, Einheiten (z.B. Stück) und Steuersätze angelegt

### Technische Voraussetzungen

*   Mindestens Shopware Version 5.7.0
*   plentymarkets
*   Shell-Zugriff (FTP ist nicht ausreichend)
*   Zugriff auf alle Konfigurationsdateien (insbesondere der <span class="c18">php.ini)
*   Zugriff auf die Crontab (mehr dazu[ ](https://www.google.com/url?q=http://man.plentymarkets.eu/tools/shopware-connector/installation/%232-4&sa=D&ust=1507645556713000&usg=AFQjCNGlNwHjHXklELIk7h0zee0xaX4JxQ)<span class="c13">[hier](https://www.google.com/url?q=http://man.plentymarkets.eu/tools/shopware-connector/installation/%232-4&sa=D&ust=1507645556713000&usg=AFQjCNGlNwHjHXklELIk7h0zee0xaX4JxQ)) // Aktivierte Cronjobs (minütlich)
*   php-cli > 7.4 Binary mit min. 512 MB RAM und unbegrenzter Prozesslaufzeit (mehr dazu[ ](https://www.google.com/url?q=http://man.plentymarkets.eu/tools/shopware-connector/installation/%232-1&sa=D&ust=1507645556714000&usg=AFQjCNHRqhkpvYZY_MT-7htcrsSKgjKUiw)<span class="c13">[hier](https://www.google.com/url?q=http://man.plentymarkets.eu/tools/shopware-connector/installation/%232-1&sa=D&ust=1507645556714000&usg=AFQjCNHRqhkpvYZY_MT-7htcrsSKgjKUiw))

Sind diese Voraussetzungen nicht erfüllt, ist ein Betrieb des Connectors unmöglich. Fehlen Ihnen darüber hinaus erweiterte Kenntnisse im Umgang mit beiden Systemen, empfehlen wir Ihnen sich an einen Systemadministrator oder Ihre betreuende Agentur zu wenden.

Möchten Sie die Einrichtung und Verwaltung des Shopware-Connectors zu Ihrem plentymarkets-System dennoch eigenverantwortlich übernehmen, beachten Sie bitte neben den oben genannten Voraussetzungen auch unbedingt die ausführliche Installationsanleitung mit Video-Guide (wird noch nachgeliefert) im plentymarkets[ ](https://www.google.com/url?q=https://docs.google.com/document/d/10mPeV3xqx4We71dYQdPmJK2qvb21Rpym6FG_tKwHKfc/edit?usp%3Dsharing&sa=D&ust=1507645556715000&usg=AFQjCNHEVvgshtaGdC-_Ba42SIi4Rk4GAg)<span class="c9">[Online-Handbuch](https://www.google.com/url?q=https://docs.google.com/document/d/10mPeV3xqx4We71dYQdPmJK2qvb21Rpym6FG_tKwHKfc/edit?usp%3Dsharing&sa=D&ust=1507645556715000&usg=AFQjCNHEVvgshtaGdC-_Ba42SIi4Rk4GAg).