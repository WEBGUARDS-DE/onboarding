# CLAUDE.md – WEBGUARDS Onboarding (öffentliche Startseite)

## Zweck des Repos

Öffentliche Startseite für neue Teammitglieder: Schritte zum GitHub-Account, Link zu einem Onboarding-Issue, Überblick über den Zugang nach der Anmeldung. Art des Repos: kleines Dokument- und Konfigurations-Repo (Jekyll-Seite für GitHub Pages), kein Anwendungscode.

## Ordnerstruktur

- `README.md` – Startseite mit drei Schritten und Zugangsübersicht. Einstieg für Inhalte.
- `_config.yml` – Jekyll-Konfiguration (Theme `jekyll-theme-cayman`, Titel, Beschreibung, Autor).
- `.github/ISSUE_TEMPLATE/onboarding.md` – Vorlage für die Anmeldung als Issue. Enthält Abfragefelder für Name, E-Mail und Rolle.

## Konventionen

- Sprache: Deutsch, Du-Anrede.
- Issue-Vorlage: Label `onboarding`, Zuweisung an den Eigentümer, Titel `[ONBOARDING] Dein Name`.
- Dateinamen: Kleinschreibung, Bindestriche.

## Schreibregeln

- Kurz und einladend. Die Seite ist öffentlich lesbar, daher nur Informationen, die jeder sehen darf.
- Keine internen Links, Kundennamen, Preise, Stammdaten oder Interna.

## Pflegeregeln

- Änderungen an `README.md` nur sachlich und ohne Verweis auf interne Repos.
- Bei Änderungen an `_config.yml` vor dem Merge prüfen, ob GitHub Pages die Seite noch baut.

## Quelle der Wahrheit

- Ablauf und Zugang: `README.md`.
- Anmeldefelder: `.github/ISSUE_TEMPLATE/onboarding.md`.

## Grenzen

- Nicht manuell ändern: `.git/`.
- Keine personenbezogenen Daten in Dateien dieses Repos schreiben.
- Das Repo ist öffentlich. Keine Zugangsdaten, Tokens oder Hinweise auf interne Systeme.

## Workflows

- Basisbranch: `main`. Änderungen als Commit auf einem Branch, dann Pull Request.
- Commit-Format und PR-Vorlage: ungeprüft.

## Stolperfallen

- Das Repo ist öffentlich, die Issue-Vorlage fragt aber Name und E-Mail ab. Eingereichte Issues sind öffentlich sichtbar. Das widerspricht dem Zweck der Datenschutzwahrung und sollte vor einer Änderung der Vorlage entschieden werden.
- Die Vorlage nennt einen Assignee `ob` als feste Zuweisung. Bei Personalwechsel anpassen.
- Die `README.md` hat keine H1-Überschrift, nur einen H2-Titel. Das Jekyll-Theme erzeugt den Seitentitel aus `_config.yml`.
