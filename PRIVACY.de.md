# Datenschutzerklärung

Diese Webanwendung sammelt nichts: keine Statistik, keine Telemetrie, keine Verfolgung, keine Werbung, keine Cookies sowie keine Skripte von Dritten. An den Entwickler oder an einen Server geht nichts. Das ganze Werkzeug läuft auf deinem Gerät.

## Was verarbeitet wird und wo es bleibt

Alles Folgende bleibt auf deinem Gerät und wird nirgendwohin hochgeladen:

- Die Datenpunkte des Scooters, über Bluetooth LE gelesen.
- Die Schlüssel und Einstellungen, die du eingibst (localKey, srand, das dpId-Schema). localKey und Schema werden nur lokal im Browser gespeichert (localStorage); srand bleibt nur für die Sitzung im Speicher.
- Ein Bluetooth-Mitschnitt, den du auswertest. Er wird vollständig in der Seite gelesen und verlässt das Gerät nie.
- Das Protokoll auf dem Bildschirm. Es lebt nur in der offenen Seite. Gerätename und ID sowie der abgeleitete Sitzungsschlüssel werden anonymisiert, Zugangsdaten oder Token werden geschwärzt, bevor etwas gespeichert, angezeigt, kopiert oder gesichert wird.

## Netzverbindungen

- **Laden der Seite:** Dein Browser holt die statischen Dateien vom Anbieter (zum Beispiel GitHub Pages). Der Anbieter sieht dabei deine IP-Adresse sowie welche Datei du abgerufen hast. Das sind die üblichen Zugriffsprotokolle. Scooter-Daten, Schlüssel oder Kommandos erreichen dabei keinen Server.
- **Bluetooth LE zum Scooter:** eine lokale Funkverbindung. Das ist keine Internetverbindung. Kommandos sowie die Antworten des Scooters laufen ausschließlich zwischen deinem Browser und dem Scooter.
- **Sonst nichts.** Die Content-Security-Policy der Seite erlaubt nur `connect-src 'self'`, die Seite kann also gar keinen anderen Server ansprechen.

## Hinweis zur Original-App

Die offizielle ISINWHEEL-App ist ein Tuya-Smart-Life-Container, der sich bei der Tuya-Cloud anmeldet, um Produkt, dpId-Schema und den geräteeigenen localKey aufzulösen. Diese Seite tut das **nicht**. Sie spricht nur über Bluetooth mit dem Scooter und braucht kein Konto; localKey und srand gibst du selbst ein.

## Kontakt

Bei Fragen zum Datenschutz wende dich an den Autor (Laufbursche) auf GitHub: https://github.com/Laufbursche42
