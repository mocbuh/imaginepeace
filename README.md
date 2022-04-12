# imaginepeace

# Deployment Schritte

Die Internetseite wird von Netlify gehosted und automatisch geupdated wenn der main branch ein neues commit erhält.

Um ein update zu machen, folgende Schritte befolgen:

1. Website updaten
2. `git add .` um alle Änderungen für das neue commit zu stagen
3. `git commit -m "Beschreibung der Änderungen"` um das commit zu machen
4. `git push` um das commit zu Github hochzuladen

Netlify sollte dann automatisch ein neues commit erkennen, und die Website dementsprechend updaten.

Sollte `git push` einen Authentifizierungsfehler haben, kann es sein dass der ssh key der bei Github hinterlegt ist, nicht in `ssh-agent` hinterlegt ist. Für diesen Fall, den key hinterlegen mit `ssh-add ~/.ssh/id_rsa`. Um zu checken ob `ssh-agent` einen key hat, einfach `ssh-add -l` ausführen.

