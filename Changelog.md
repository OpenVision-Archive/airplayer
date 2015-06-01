## 0.3.1 ##
  * AzBox fixes
  * Bildschirmschoner bei Audio-Streaming
  * Box kann bei Audio-Streaming aus dem StandBy aufgeweckt werden
  * neuer Lokaler Proxy (Premium-Feature) Videos werden lokal zwischengespeichert, dies verbessert die Wiedergabe und ermöglicht auch die Wiedergabe von m3u8-Streams (MyVideo, ZDF, AirVideo etc).
  * Überarbeitetes update Konzept
  * Verbesserung der Stabilität
  * Fehlerbehebungen

## 0.2.4 ##
  * Fehlerbehebung

## 0.2.3 ##
  * Verbesserungen für Aduio-Streaming unter oe1.6
  * Steuern der Alutstärke beim Audio-Streaming über das iOS Device
  * Verbesserungen der Stabilität

## 0.2.2 ##
  * Fehlerbehebung für das Audio-Streaming unter oe1.6 auf Dreamboxen

## 0.2.1 ##
  * Setzen der Downmix Option für Audio-Streaming
  * Fehler beim Starten/Stoppen behoben
  * Verwenden der Architekturinformationen für das Auto-Update

## 0.2.0 ##
  * AirTunes Audio-Streaming hinzugefügt
  * Playback-Status wird an das iOS Device zurückgemeldet
  * TV-Bild kann bei der Wiedergabe von Fotos gestoppt werden
  * Blockieren von Frontends durch zeroconfig behoben
  * Fehlerbehebung

## 0.1.10 ##
  * bug in der Fehlerbehandlung beseitigt.

## 0.1.9 ##
  * Lokaler cache für langsame Internetverbindungen hinzugefügt
> > Wenn ein Stream ruckelt, einfach die RECORD taste drücken. Der Download startet und der Downloadfortschritt ist in der InfoBar zu sehen.
> > Forstsetzen des Playbacks über die PLAY taste.
  * Fehlerbehandlung verbessert

## 0.1.8 ##
  * hoffentlich den bug mit dem MediaPlayer beseitigt
  * Update Prozess verbesser
  * kleinere bugfixe

## 0.1.7 ##
  * [InfoBar](InfoBar.md) zum [MoviePlayer](MoviePlayer.md) hinzuegefügt mit Anzeige des Bufferfüllstandes
  * Update check hinzugefügt. Prüft automatisch ob Updates verfügbar sind. Diese Updates können direkt über das Plugin geladen und ausgeführt werden. Ein changelog wird ebenfalls vor dem Update angezeigt.
  * BufferControl für vu+ boxen deaktiviert
  * kleinere verbesserungen im playback handling

## 0.1.6 ##
  * Bilder von Android mit Doubletwist und Airsync können nun angezeigt werden
  * neue Option zum verwenden eines QuickTime userAgents (nötig z.B. für AppleTrailer)
  * Verarbeitung von QuickTime weiterleitungen. (Apple Trailer in SD oder z.B. die Special events von der Apple seite schickt ein link zu einer mov datei, die aber nur ein paar bytes enthält. in der datei sind die richtigen links zum streamen der videos! GStreamer kann damit aber nicht umgehen. Daher werden diese Dateien nun vom plugin gelesen und ausgewertet sofern der link mov enthält und die datei unter 10kb ist. Von meinem iPad gehen nun die Apple Trailer und special events von der Aplle Seite)

## 0.1.5b ##
  * fehler beim starten behoben bei falscher typenkonvertierung

## 0.1.5 ##
  * vom iPhone/iPad übermittelte Startposition auswerten und setzen (durch das springen beim starten wurden bei mir die probleme mit dem ruckeln am anfang wesentlich besser)
  * beenden von alten zeroconfig instanzen vor dem straten einer neuen
  * deaktivierung einiger debug ausgaben

## 0.1.4 ##
  * die Liste mit den Netzwerk devices in den Settings wird jetzt automatisch mit den vorhandenen Interfaces bestückt! (Behebt hoffentlich das Problem mit den verschiedenen Namen der WLAN geräte)
  * Neue Option zum einstellen des Buffers für gstreamer. Das verbessert hoffentlich an einigen Stellen Probleme mit ruckeln. Der Buffer hatte vorher 1MB, default ist jetzt 8MB, Maximale Größe ist mir nicht bekannt, möglicherweise führt ein zu großer Wert zu Fehlern.
  * Buffer Control: Beim starten eines Videos sollte das Video automatisch auf Pause springen, bis der Buffer ca 90% gefüllt ist, dann beginnt automatisch das Abspielen. Fällt der buffer auf unter 3% Füllstatus wird wieder pausiert und gewartet bis der Buffer wieder ca 90% gefüllt wurde. Das ganze kann per fernbedienung der Box übersteuert werden

## 0.1.3 ##
  * cleanups
  * kleine änderungen an zeroconfig hoffentlich geht damit auch wlan

## 0.1.2 ##
  * bugfixing

## 0.1.1 ##
  * GUI hinzugefügt

## 0.1.0 ##
  * Erstes Release