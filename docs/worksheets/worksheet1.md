# Arbeitsblatt: Einheit 1 – Einführung in Docker und Containerisierung

## Lernziele
- Verstehen, was Docker ist und warum Containerisierung wichtig ist.
- Docker auf dem eigenen System installieren.
- Grundlegende Docker-Konzepte wie Images, Container und die Docker Engine verstehen.

---

## 1. Was ist Docker?

Docker ist eine Open-Source-Plattform, die Entwicklern hilft, Anwendungen in **Containern** zu erstellen, bereitzustellen und zu verwalten. Container sind leichtgewichtige, isolierte Umgebungen, die alle notwendigen Abhängigkeiten enthalten, um eine Anwendung konsistent auf verschiedenen Systemen auszuführen.

### Vorteile der Containerisierung:
- **Portabilität:** Container können auf verschiedenen Systemen unverändert ausgeführt werden.
- **Effizienz:** Container nutzen den Kernel des Host-Betriebssystems, sind daher ressourcenschonender als virtuelle Maschinen.
- **Isolierung:** Anwendungen in Containern laufen isoliert und beeinflussen sich nicht gegenseitig.

---

## 2. Docker-Architektur

Docker besteht aus verschiedenen Hauptkomponenten:
- **Docker Engine:** Die zentrale Komponente, die Container erstellt und verwaltet.
- **Docker Image:** Eine Vorlage, die alle für eine Anwendung benötigten Dateien enthält.
- **Docker Container:** Eine Instanz eines Images, die isoliert auf dem Host-System läuft.

---

## 3. Installation von Docker

### Schritt-für-Schritt-Anleitung:

#### Für Windows und MacOS:
1. Besuchen Sie die Seite [https://www.docker.com/get-started](https://www.docker.com/get-started).
2. Laden Sie Docker Desktop herunter und installieren Sie es.
3. Starten Sie Docker nach der Installation.

#### Für Linux:
1. Öffnen Sie ein Terminal.
2. Führen Sie folgende Befehle aus:
   ```bash
   sudo apt-get update
   sudo apt-get install docker-ce docker-ce-cli containerd.io
   ```bash
3. Überprüfen Sie die Installation mit:
   ```bash
   docker --version
   ```

---

# 4. Grundlegende Docker-Konzepte

## 4.1 Docker-Images
Docker-Images sind unveränderliche Vorlagen, die alle Komponenten einer Anwendung enthalten (z.B. Code, Laufzeitumgebung, Bibliotheken).
Entwickler können auf [Docker Hub](https://hub.docker.com) nach offiziellen oder benutzerdefinierten Images suchen.

## 4.2 Docker-Container
Container sind laufende Instanzen von Docker-Images.
Container sind isolierte Umgebungen, in denen Anwendungen unabhängig voneinander ausgeführt werden.

---

# 5. Docker-Befehle: Erste Schritte

Hier sind einige grundlegende Docker-Befehle:

### docker run
Startet einen Container basierend auf einem Image.

Beispiel:
```bash
docker run hello-world
```


### docker ps
Zeigt eine Liste der aktuell laufenden Container.

```bash
docker ps
```


### docker stop
Stoppt einen laufenden Container.

```bash
docker stop <container_id>
```

---

# 6. Praxisaufgabe

## Aufgabe 1: Erster Docker-Container
Starten Sie einen "Hello World"-Container.
**Frage:** Was sehen Sie in der Ausgabe? Beschreiben Sie die Ergebnisse.

## Aufgabe 2: Docker Hub durchsuchen
1. Besuchen Sie [Docker Hub](https://hub.docker.com).
2. Suchen Sie nach einem Image für **Node.js** oder **Python**.
3. **Frage:** Notieren Sie den Namen des Images und lesen Sie die Beschreibung.

---

# 7. Reflexionsfragen
- Was ist der Vorteil von Containern gegenüber virtuellen Maschinen?
- Warum ist die Konsistenz von Anwendungen in verschiedenen Umgebungen wichtig?
- Welche Herausforderungen könnten bei der Verwendung von Containern auftreten?

---

**Vorschau:** In der nächsten Einheit beschäftigen wir uns mit Docker-Images und dem Erstellen von eigenen Containern.
