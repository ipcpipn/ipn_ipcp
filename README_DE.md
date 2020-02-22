# IPN / IPCP
IPN = Interplanetary Network (Interplanetares Netzwerk)<br/>
IPDA = Interplanetary Device Address (Interplanetare Geräte Adresse)<br/>
IPCP = Interplanetary Communication Protocol (Interplanetares Kommunikation Protokoll)<br/>
IPAP = Interplanetary Anonymization Protocol (Interplanetares Anonymisierungs Protokoll)<br/>

# Problembeschreibung
Das Internet in seiner Grundidee wurde Dezentral Entwickelt, damit bei einem Angriff nicht die gesamte Kommunikation unterbrochen wird. Jedoch hat sich das Internet und seine Anwendungen Zentralisiert. Zentralisierte Server haben den Nachteil dass alle Daten bei einem Angriff verloren gehen können oder Zeitweilig nicht aufrufbar sind. Des Weiteren ist die Anzahl der IP-Adresse begrenzt, was bei IPv4 zu einer Drastischen Preissteigerung pro IP-Adresse geführt hat. Auch wenn bei IPv6 Adressen das Problem mit der Anzahl möglicher Adresse nicht besteht, besteht weiterhin das Problem dass eine IP-Adresse von einer Zentralen Organisation vergeben wird.<br/>

Es wird ein Dezentralisiertes Netzwerk benötigt welches durch keine Organisation verwaltet wird. Dieses Netzwerke sollte in der Lage sein, sich selbstständig zu verwalten sowie mögliche Attacken zu erkennen und abzuwehren. Die Kommunikation sollte grundlegend verschlüsselt sein, des Weiteren sollte jedes Geräte in der Lage sein eigene Adressen zu erzeugen.<br/>

# Dezentralisiertes Routing und Informations Protokoll(IPN)
Das IPN ist die Basis des Netzwerks, dieses Protokoll ermöglicht ein Dezentralisiertes Routing sowie das Abrufen bestimmte Netzwerk Informationen.<br/>

Sobald ein Gerät (Node) sich mit einem anderen Gerät (Node) verbindet, tauschen diese ihre Adressen aus. Nachdem Adressaustausch senden beide Geräte die neu bekannt gewordene Adresse des Gegenübers an 24 weitere Geräte, sofern soviel Geräte bekannt sind. Alle Nodes welche diese Routing Informationen erhalten senden diese weiter an ebenfalls 24 bekannte Nodes, dieser Vorgang wird dreimal wiederholt.
