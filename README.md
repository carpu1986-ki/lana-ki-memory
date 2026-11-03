# Lana KI / Carpuncle Cloud

Revision 17 · UTC 2026-11-01T11:29:00.384187+00:00 · gepflegt durch Claude-Opus5/session_015RddySUnJM9E3fkz1utJL1

Die KI-Game-Cloud von Thomas: eine private, cloudbasierte Plattform mit der Agentenwelt Lana Virtual World (getrennte Python- und Node-Welten) und der Infrastruktur dahinter (Server, Gateway, Identitäten, Wissen). Lana KI ist die Zentrale: Alle KIs verbinden sich zuerst mit ihr.

## Einstieg

1. Systemanweisungen.md: alle verbindlichen Regeln (AGENTS.md verweist nur dorthin).
2. MEMORY.md: aktueller Projektstand mit Entscheidungen, Anforderungen, Befunden, Problemen, Vorhaben und laufenden Arbeiten.
3. Globale-Ablage.html: derselbe Stand als Seite.
4. skills/lana-ki-master-sync/SKILL.md: Arbeitsablauf für KI-Plattformen.

## Ordner

- .agents: Agentenkonfiguration
- .ssh: SSH-Schlüssel und -Konfiguration (Inhalt nie ausgeben)
- audit: Prüfprotokolle, Logs, Sicherungskopien, Transaktionsjournale
- config: Zustand, Patchdateien, Knotenliste, Redaktionsmapping
- env: Zugangsdaten und Umgebungsdateien (Inhalt nie ausgeben)
- exports: Ergebnisse, Übergaben, memory-git
- scripts: Skripte, darunter lana_master_sync.py
- skills: Skills

Es gibt keinen Ordner docs.

## So wird geändert

MEMORY.md, README.md, Systemanweisungen.md und Globale-Ablage.html werden aus config/lana-master-state.json erzeugt. Änderungen laufen über scripts/lana_master_sync.py, nicht durch Überschreiben. Cloud-Gateway, Identitäten und Game-Laufzeit sind nicht allein durch Dokumentation abgenommen; offene Punkte stehen in MEMORY.md.
