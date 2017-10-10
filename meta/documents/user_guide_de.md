![plentymarkets Logo](http://www.plentymarkets.eu/layout/pm/images/logo/plentymarkets-logo.jpg)

# PlentyConnector plugin Shopware

## <span class="c8">Produktinformationen

Bitte beachten:

Die Shopware Connector Version ab 2.0 (PSC7) ist ausschließlich für plentymarkets 7 geeignet! Bitte führen Sie kein Update des Connectors auf diese Version mit plentymarkets 6 durch.

Der neue plentymarkets Shopware Connector (PSC7) wurde durch unseren Expert Partner arvatis media entwickelt. Der neu entwickelte Connector bietet eine Vielzahl erweiterter Möglichkeiten für einen besseren und schnelleren Abgleich - als Basis dient die moderne REST-API.

Nutzen Sie jetzt alle Vorteile des neuen plentymarkets 7 und der aktuellsten Shopware Version für die optimale eCommerce-Synergie aus Warenwirtschaft und individualisiertem Shop.

### Neuen Funktionen / neue Abgleiche des Connectors

Während der alte Connector teilweise nur sehr eingeschränkt abgeglichen hat, überträgt der neue Connector alle Felder, inklusive der Meta-Daten - ein Umweg über Freitextfelder oder eine Nachpflege in Shopware ist nicht mehr nötig

Auch die Fehlertoleranz wurde deutlich erhöht. So wird ein Abgleich bei einem Fehler nicht direkt abgebrochen, sondern mit den nächsten Positionen weiter durchgeführt.

Es findet ein Merge anstelle des initialen Exports statt. Dadurch können beispielsweise Kategorien oder Artikel angelegt und editiert werden, ohne dass es beim Abgleich zu einem Problem kommt.

Für eine detaillierte Auflistung möchten wir gerne auf das ausführliche[ ](https://www.google.com/url?q=https://docs.google.com/document/d/10mPeV3xqx4We71dYQdPmJK2qvb21Rpym6FG_tKwHKfc/edit?usp%3Dsharing&sa=D&ust=1507645556705000&usg=AFQjCNFBKAe5FIQiGcXF9GA-z2Uud2MKmQ)<span class="c9">[Handbuch vom PSC7](https://www.google.com/url?q=https://docs.google.com/document/d/10mPeV3xqx4We71dYQdPmJK2qvb21Rpym6FG_tKwHKfc/edit?usp%3Dsharing&sa=D&ust=1507645556706000&usg=AFQjCNEVv48pBAe8ezFN7q5-XRZZma-FXA) verweisen.

Die arvatis media wird als betreuende Agentur ebenfalls einfache Supportfragen im[ ](https://www.google.com/url?q=https://forum.plentymarkets.com/c/shopware-connector&sa=D&ust=1507645556707000&usg=AFQjCNE_enSGlva-gtn1hLPZX90WtAVquA)<span class="c9">[Connector Forum](https://www.google.com/url?q=https://forum.plentymarkets.com/c/shopware-connector&sa=D&ust=1507645556707000&usg=AFQjCNE_enSGlva-gtn1hLPZX90WtAVquA) beantworten und freut sich jederzeit über konstruktive Kritik und weitere Anregungen zur fortlaufenden Optimierung.

Darüber hinaus erlaubt die modulare Opensource Gestaltung des neuen Connectors ebenfalls die individuelle Weiterentwicklung des Connectors oder die Bereitstellung neuer Funktionen für die Community über das[ ](https://www.google.com/url?q=https://github.com/plentymarkets/plentymarkets-shopware-connector/branches&sa=D&ust=1507645556708000&usg=AFQjCNF3KInI2eUu3AdOgvbt6eIPUjqjtg)<span class="c9">[GitHub Projekt](https://www.google.com/url?q=https://github.com/plentymarkets/plentymarkets-shopware-connector/branches&sa=D&ust=1507645556709000&usg=AFQjCNEc8D9qxJkLBgMuIuZbCvJZSSUOXg).

## <span class="c8">Installationsanleitung

Für die Einrichtung Ihrer plentymarkets 7 und Shopware-Anbindung sind einige wichtige Voraussetzungen zwingend erforderlich, um eine dauerhaft reibungslose Synchronisation der Daten beider Systeme zu gewährleisten,

### Systemvoraussetzungen

*   plentymarkets-Version 7.0
*   mindestens Shopware-Version 5.2.22
*   Ein für Shopware eingerichteter Mandant in plentymarkets
*   <span class="c11">In Shopware sind alle benötigten Kundengruppen, Einheiten (z.B. Stück) und Steuersätze angelegt
*   Bei einer vorherigen Migration von plentymarkets Version 6 zu Version 7:

*   <span class="c11">Die Kategoriestruktur, Preise, Artikel sind nach der Migration in Plentymarkets bereinigt und überprüft worden. Und können so in das Shopware System übertragen werden.
*   Keine Aufträge in Shopware mit dem Auftragsstatus “Offen”, die durch den alten Connector bereits zu plentymarkets übertragen wurden

### Technische Voraussetzungen

*   Mindestens Shopware Version 5.2.22
*   plentymarkets Version 7
*   Shell-Zugriff (FTP ist nicht ausreichend)
*   Zugriff auf alle Konfigurationsdateien (insbesondere der <span class="c18">php.ini)
*   Zugriff auf die Crontab (mehr dazu[ ](https://www.google.com/url?q=http://man.plentymarkets.eu/tools/shopware-connector/installation/%232-4&sa=D&ust=1507645556713000&usg=AFQjCNGlNwHjHXklELIk7h0zee0xaX4JxQ)<span class="c13">[hier](https://www.google.com/url?q=http://man.plentymarkets.eu/tools/shopware-connector/installation/%232-4&sa=D&ust=1507645556713000&usg=AFQjCNGlNwHjHXklELIk7h0zee0xaX4JxQ)) // Aktivierte Cronjobs (minütlich)
*   php-cli > 7.0 Binary mit min. 512 MB RAM und unbegrenzter Prozesslaufzeit (mehr dazu[ ](https://www.google.com/url?q=http://man.plentymarkets.eu/tools/shopware-connector/installation/%232-1&sa=D&ust=1507645556714000&usg=AFQjCNHRqhkpvYZY_MT-7htcrsSKgjKUiw)<span class="c13">[hier](https://www.google.com/url?q=http://man.plentymarkets.eu/tools/shopware-connector/installation/%232-1&sa=D&ust=1507645556714000&usg=AFQjCNHRqhkpvYZY_MT-7htcrsSKgjKUiw))

Sind diese Voraussetzungen nicht erfüllt, ist ein Betrieb des Connectors unmöglich. Fehlen Ihnen darüber hinaus erweiterte Kenntnisse im Umgang mit beiden Systemen, empfehlen wir Ihnen sich an einen Systemadministrator oder Ihre betreuende Agentur zu wenden.

Möchten Sie die Einrichtung und Verwaltung des Shopware-Connectors zu Ihrem plentymarkets-System dennoch eigenverantwortlich übernehmen, beachten Sie bitte neben den oben genannten Voraussetzungen auch unbedingt die ausführliche Installationsanleitung mit Video-Guide (wird noch nachgeliefert) im plentymarkets[ ](https://www.google.com/url?q=https://docs.google.com/document/d/10mPeV3xqx4We71dYQdPmJK2qvb21Rpym6FG_tKwHKfc/edit?usp%3Dsharing&sa=D&ust=1507645556715000&usg=AFQjCNHEVvgshtaGdC-_Ba42SIi4Rk4GAg)<span class="c9">[Online-Handbuch](https://www.google.com/url?q=https://docs.google.com/document/d/10mPeV3xqx4We71dYQdPmJK2qvb21Rpym6FG_tKwHKfc/edit?usp%3Dsharing&sa=D&ust=1507645556715000&usg=AFQjCNHEVvgshtaGdC-_Ba42SIi4Rk4GAg).