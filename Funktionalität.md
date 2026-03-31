### Funktionalität
Das System ist ein am Handgelenk tragbares Wearable zur kontinuierlichen Erfassung von Vital- und Bewegungsdaten im Alltag. Es dient der Erhebung von Daten zur Herzfrequenz, Sauerstoffsättigung sowie Bewegungsinformationen des Nutzers.
Die erfassten Daten werden drahtlos an ein externes Endgerät, beispielsweise ein Smartphone, übertragen und dort gespeichert. Das Wearable selbst verfügt über keine Anzeige- oder Bedienelemente und arbeitet vollständig autonom im Hintergrund.
Das System ist für den täglichen Einsatz über eine typische Nutzungsdauer von 12 Stunden ausgelegt und für wiederholte Ladezyklen konzipiert.  Es ist für den Einsatz im Alltag geeignet und gegenüber äußeren Einflüssen wie Feuchtigkeit geschützt, sodass ein Betrieb auch bei Kontakt mit Wasser möglich ist.
Die Funktionalität basiert auf dem Zusammenspiel von Sensorik, zentraler Verarbeitungseinheit, Energieversorgung und drahtloser Kommunikation, wie in der Systemarchitektur dargestellt.
#### Grundlegender Ablauf
Das Wearable erfasst kontinuierlich Daten des Nutzers, verarbeitet diese intern und überträgt sie anschließend drahtlos an ein externes System. Eine zentrale Recheneinheit steuert dabei alle Abläufe innerhalb des Systems.
#### Datenerfassung
Die Erfassung der Nutzerdaten erfolgt über zwei zentrale Sensor Komponenten.
Ein Pulsoximeter erfasst Daten auf optischem Wege, sodass die Herzfrequenz sowie die Sauerstoffsättigung des Blutes berechnet werden können. Dazu wird Licht in die Haut eingestrahlt und die Reflexion des Lichts durch das Blut analysiert. Durch die periodischen Änderungen des Blutvolumens infolge des Herzschlags kann die Herzfrequenz bestimmt werden. Gleichzeitig ermöglicht die unterschiedliche Absorption von Licht die Abschätzung der Sauerstoffsättigung.
Die Messung erfolgt in regelmäßigen Intervallen und liefert diskrete Vitaldaten.
Zusätzlich erfasst eine Inertiale Messeinheit (IMU) kontinuierlich Bewegungsdaten. Diese misst lineare Beschleunigungen sowie Rotationsbewegungen in allen drei Raumachsen. Dadurch können sowohl Bewegungen als auch Lageänderungen des Handgelenks erfasst werden.
Die Sensoren sind direkt an die zentrale Verarbeitungseinheit angebunden und liefern ihre Messwerte fortlaufend an das System.
#### Datenverarbeitung
Die Verarbeitung der Sensordaten erfolgt durch den Mikrocontroller, der als zentrale Steuereinheit des Systems fungiert.
Er übernimmt das Auslesen der Sensordaten, deren zeitliche Zuordnung sowie die strukturierte Aufbereitung. Alle Daten werden mit Zeitstempel versehen, um eine spätere Auswertung zu ermöglichen.
Das System ist so ausgelegt, dass die Datenverarbeitung kontinuierlich erfolgt und keine Unterbrechungen im Datenfluss entstehen. Bei Bedarf werden Daten temporär gespeichert.
#### Datenübertragung
Die aufbereiteten Daten werden drahtlos über eine integrierte Kommunikationseinheit an ein externes Endgerät, beispielsweise ein Smartphone, übertragen.
Daten werden im Mikrokontroller temporär zwischengespeichert und für die Übertragung zum Server verarbeitet. Es wird sichergestellt, dass alle erfassten Daten vollständig und ohne Verlust und mit Timestamps übertragen werden. Bei temporären Verbindungsunterbrechungen erfolgt eine Zwischenspeicherung im System.
#### Energieversorgung
Die Energieversorgung des Systems erfolgt über einen wiederaufladbaren Akku. Dieser ermöglicht einen kontinuierlichen Betrieb über einen typischen Nutzungstag von 12 Stunden. Die Aufladung erfolgt über einen kabelgebundenen Anschluss mit integrierter Spannungsanpassung sowie Schutzmechanismen gegen Überladung.
Zur Sicherstellung eines stabilen Betriebs werden die einzelnen Komponenten mit den jeweils benötigten Spannungen versorgt. Die Energieverteilung ist so ausgelegt, dass ein effizienter und zuverlässiger Betrieb gewährleistet ist. Zusätzlich sind Schutzmechanismen gegen Über- und Tiefentladung integriert, um die Lebensdauer des Akkus zu erhöhen und die Betriebssicherheit zu gewährleisten.

### Glossar 
#### Wearable: 
nicht obstruktives Tragen am Körper getragen werden ohne Einschränkung von Körperfunktionen
An- und ablegbar durch die benutzende Person
Integrieren und Kombinieren Sensorik, Datenverarbeitung und Kommunikation

