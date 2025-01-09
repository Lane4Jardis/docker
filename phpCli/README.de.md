# Lane4 Digital PHP CLI

![Build Status](https://github.com/lane4jardis/docker/actions/workflows/phpCli.yml/badge.svg)
[![Docker Image Version](https://img.shields.io/docker/v/lane4jardis/phpcli?sort=semver)](https://hub.docker.com/r/lane4jardis/phpcli)

### Bereitstellung von versionierten PHP Docker Images für Konsolenanwendungen

Das **Lane4 PHP CLI** Tool dient zur Bereitstellung plattformübergreifender PHP-CLI Docker Images. Es unterstützt PHP-Versionen von **7.4 bis 8.3** und ermöglicht Entwicklern sowie Administratoren, konsistente und zuverlässige Umgebungen für ihre Konsolenanwendungen zu erstellen und zu betreiben.

Unsere Docker Images sind sowohl für **AMD64** als auch für **ARM64** Architekturen verfügbar und werden auf [Docker Hub](https://hub.docker.com/r/lane4jardis/phpcli) bereitgestellt. Dies gewährleistet eine breite Kompatibilität und ermöglicht den Einsatz auf verschiedenen Hardware-Plattformen, einschließlich moderner Server und IoT-Geräte.

### Es wurden folgende Komponenten angewendet:
 - alpine 7.4 - 8.3 Basis Image
 - xdebug
 - pdo
 - mysql
 - redis
 - curl
 - dom
 - soap
 - zip
 - mbstring

### Image Größe
- 100MB and 107MB :-)

## Voraussetzungen

Beachten Sie bitte die Voraussetzungen zur Installation aus den Informationen der README.md im Docker Projekt Root Verzechnis.

### Verwendung

Wir haben ein Makefile erstellt, welches dir über den Befehl `make` auf der Konsole alle Möglichkeiten zur Verwendung anbietet.


### Anpassung für eigene Zwecke

Falls Sie das Tool vollständig an Ihre eigenen Anforderungen anpassen möchten, bearbeiten Sie bitte die entsprechenden Einträge in der `.env`-Datei.

Dies ermöglicht eine flexible Konfiguration der bereitgestellten Docker Images, einschließlich spezifischer PHP-Erweiterungen, Konfigurationseinstellungen und weiterer Anpassungen.

Für diese Art der Verwendung benötigst du dann ein eigenes Source und Image Repository.

Es würde uns in diesem Fall sehr freuen, wenn du uns als Unterstützer Deiner Docker Images erwähnen würdest.


## Lieferumfang von `phpCli`

Das `phpCli`-Paket umfasst die folgenden Komponenten:

- **Source Files**:
    - `/phpcli` – Enthält den Quellcode und die Konfigurationsdateien für das PHP-CLI Tool.

- **Support Dateien**:
    - `.env` – Umgebungsvariablen zur Konfiguration der Docker Images.
    - `docker-compose.yml` – Docker Compose Konfigurationsdatei zur Orchestrierung der Container.
    - `Dockerfile` – Dockerfile zur Erstellung der PHP-CLI Images.
    - `Makefile` – Einfache Kommandozeilenhilfe. Rufen Sie `make` in der Konsole auf, um verfügbare Befehle anzuzeigen.
    - `.github/workflows/phpCli.yml` – GitHub Actions Workflow zur Automatisierung von Builds und Tests.

- **Dokumentation**:
    - `README.md` – Ausführliche Dokumentation und Anleitungen zur Nutzung des Tools.
