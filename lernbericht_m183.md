# Lern-Bericht M133
## Einleitung

In diesem Modul geht es um die Arbeit mit JSF, xhtml und css um Webapplikationen zu erstellen.

## Was habe ich gelernt?

Ich habe gelernt wie man die ID einer Sitzung ausgeben kann als String.

## Beschreibung

Um die Session ID als String auszugeben, muss man in Java eine getSessionID() Klasse erstellen, welche mit den Befehlen:
FacesContext fCtx = FacesContext.getCurrentInstance(); und
HttpSession session = (HttpSession) fCtx.getExternalContext().getSession(false);, die aktuelle SessionID herausfindet.
Danach gibt man die ID zurück mithilfe von: return session.getID(); , und schliesslich kann man im ".xhtml" File diese ID in einem Text mit #{*JavaKlassen-Name*.sessionId}.

![image](https://user-images.githubusercontent.com/47601770/187220491-08fd586e-c2be-4142-9ac7-2c968960b81d.png)

Code Snippet:
```
public String getSessionId() {
        FacesContext fCtx = FacesContext.getCurrentInstance();
        HttpSession session = (HttpSession) fCtx.getExternalContext().getSession(false);
        return session.getId();
    }
```

## Verifikation

Im Screenshot sehen wir die beiden Teile des Codes und zu unterst auch die Ausgabe der SessionID.
Die Java Klasse ist auch als Snippet vorhanden.

# Reflektion zum Arbeitsprozess

Ich finde es ist schlau gehandelt und es war einer der ersten Male, wo ich erfolgreich Java mit HTML kombinieren konnte.

Ich habe leider spät bemerkt, dass die Abgabe nicht spät am Abend ist sondern Mittagszeit, wegen der Teamsnachricht, weshalb ich leider das Portfolio verspätet abgebe.

**Für nächstes Mal muss ich mehr auf die vorgegebenen Zeiten achten** 
