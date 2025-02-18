# Modul-210


# HTML Docker App

Dieses Projekt enthält eine einfache HTML-Anwendung, die in einem Docker-Container ausgeführt wird. Hier sind die Schritte, um das Docker-Image zu erstellen, zu pushen und den Container zu starten.

## 1. Docker-Image erstellen

Um das Docker-Image zu erstellen, führe den folgenden Befehl aus:

```bash
docker build -f Dockerfile -t ghcr.io/arlindlind/html-docker-app:latest .
```

## 2. Docker-Image pushen

Um das erstellte Docker-Image auf GitHub Container Registry zu pushen, verwende diesen Befehl:

```bash
docker push ghcr.io/arlindlind/html-docker-app:latest
```

Ersetze `<githubusername>` mit deinem GitHub-Benutzernamen.

## 3. Container starten

Um den Docker-Container im Hintergrund zu starten und ihn auf Port 8080 verfügbar zu machen, führe diesen Befehl aus:

```bash
docker run -d -p 8080:80 --name html-docker-app ghcr.io/arlindlind/html-docker-app
```

Ersetze `<githubusername>` mit deinem GitHub-Benutzernamen.

## 4. Container stoppen

Wenn du den laufenden Container stoppen möchtest, kannst du den folgenden Befehl verwenden:

```bash
docker stop html-docker-app
```

## 5. Container löschen

Um den gestoppten Container zu löschen, führe diesen Befehl aus:

```bash
docker rm html-docker-app
```

## 6. Docker-Image löschen

Wenn du das Docker-Image löschen möchtest, verwende den folgenden Befehl:

```bash
docker rmi ghcr.io/arlindlind/html-docker-app:latest
```

Ersetze `<githubusername>` mit deinem GitHub-Benutzernamen.
