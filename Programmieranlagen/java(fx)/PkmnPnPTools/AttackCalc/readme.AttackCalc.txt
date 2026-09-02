Dies ist ein DmgCalculator für Pokemon, welcher zwar auch für die offiziellen Spiele funktioniert,
aber primär für mein Pokemon-PnP ausgelegt ist.

Als ich in der letzten Woche meines 3-wöchigen Programmierunterrichts gelernt habe was Objekte sind und wie man sie initialisiert, 
habe ich um das gelernte zu verinnerlichen und zu erproben dieses Programm geschrieben.
Ich habe auch versucht das MVC-Pattern zu befolgen, bin aber nicht ganz zufrieden, inwieweit ich das geschafft habe.

In PkmnObjekt.CreatePkmnObjectForBattletools werden Pokemon-Objekte initialisiert, 
unteranderem über die BattletoolsDM.Daten_Kampfteilnehmer und StatCalc.Pkmn_Liste_Import als Grundlage.
Diese Objekte bieten die Starteinstellungen für das Programm.

Im Overlay kann ein Angreifer und beliebig viele Verteidiger gewählt werden.
Die Art des Angriffs kann spezifiziert werden und am Ende über "Show" wird eine Tabelle ausgegeben, 
welche anzeigt welches getroffene Pokemon wie viel Schaden erhällt.
Dabei werden die Typenwechselwirkungen berücksichtigt und Felder offen gelassen, 
um aus dem PnP Spiel Einfluss auf die Rechnung nehmen zu können.

Die einzelnen Objekte lassen sich jeweils editieren, falls Daten nicht vollständig waren 
oder sich während des Spiels geändert haben.
Der Button "get Data" gibt in die Konsole alle Daten zu allen Objekten aus. 
Einmal gut lesbar und einmal in der korekten Formatierung um sie in die Arrays einzukopieren, welche die Starteinstellungen aufbauen.
----------------------------------------------------------------------------------------------------------------------------------------

Zuerst habe ich in Exel den groben Aufbau des Overlays dargelegt und markiert wo welche Kontrollelemente liegen sollen.
Dann habe ich einen befreundeten DM (welcher später das Programm selbst benutzen will) konsultiert und Vorschläge eingeholt.
Wie man sieht, habe ich aufgrund der Vorschläge einiges geändert.

Wenn ich an dem Programm in Zukunft weiter arbeite, möchte ich die Buttonfunktionsbelegung über eine for-schleife belegen um Code-Wiederholung zu vermeiden.
Ich kam noch nicht um die resultierenden Fehler dabei herum.
Ich möchte tracken welches Pokemon wie viel HP hat und Death-saves integrieren.
Insgesamt eine Fusion aus AngriffsCalc, Initmap und HPTracking wäre das Ziel.
