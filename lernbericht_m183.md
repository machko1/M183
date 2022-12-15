# Lern-Bericht M183
## Einleitung

In diesem Modul haben wir die Applikationssicherheit angeschaut und die verschiedenen Lücken, welche Hackers bei einer Website/Applikation ausnutzen können. In dem Auftrag sehen was eine XSS Injection ist und wie man sie vorbeugt.

## Was habe ich gelernt?

Ich habe gelernt wie man eine XSS Injection tätigt und wie man diese im Code vorbeugen kann. 

## Beschreibung

Unter XSS meint man den Begriff "Cross Side Scripting". Dies ist das einschleusen von Scripts die Dinge ausführen auf Websites, welche ein Hacker ausnutzen kann. Um dies zu umgehen, verwendet man Escaping, was Sonderzeichen wie "<" oder "&" nicht direkt als Tags liest und so keine Befehle mehr ausgeführt werden. Man unterscheidet zwischen reflektiertes- (direkter Angriff auf Seite), und persistentes XSS (Script wird auf Seite gespeichert und anderen Benutzern angezeigt). In JSF wird immer "escaped" indem man am Ende einer Line Code: (escape="true") angibt.

![Demo183](https://user-images.githubusercontent.com/47601770/207857988-ee89de02-449c-4bf4-978b-774484c0f4fb.gif)


Code Snippet:
```
   <div class="panel-body">
        <h:outputText value="#{newsitem.detail}" escape="false"/>
   </div> 
```
escape:"true" würde diesen Fehler beheben!

## Verifikation

Im GIF wird gezeigt wie ein einfacher alert mit <script> Tags ausgeführt wird und der Pop-Up auf der Site angezeigt wird. Der Code Snippet zeigt auch wo im Code das escaping ausgeschaltet ist und wo man es ändern könnte.

# Reflektion zum Arbeitsprozess

👍 Ich habe relativ schnell das Prinzip von Cross Side Scripting verstanden und anwenden können.

👎 Ich habe das Word Dokument nicht ganz durchgearbeitet und habe nur die interessanten "praktischen" Aufgaben durchgearbeitet.


**Für das nächste Mal nehme ich mir vor, alle Word Dokumente von Aufgabe zu Aufgabe durchzuarbeiten, ausser es wird uns anders mitgeteilt! ** 
