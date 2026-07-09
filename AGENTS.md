# nuresearch — Repository-Arbeitsanweisung (AGENTS.md)

Dieses Repository ist der **verbindliche Ablageort für alle Rechercheergebnisse** von nuresearch.

## Verbindliche Regel für Agenten

Jedes **fertige** Rechercheergebnis wird als **Markdown-Datei in diesem Repository** abgelegt und nach `origin/main` **committet und gepusht** — zusätzlich zum Setzen des Issue-Status in Paperclip.

1. Lege das Dokument unter `research/` ab. Dateiname: `research/YYYY-MM-DD-<kurzes-thema-in-kebab-case>.md`.
2. Beginne mit einem YAML-Frontmatter und danach dem strukturierten Inhalt (Executive Summary zuerst, saubere Quellenangaben, klare Trennung Fakt/Annahme — gemäß deiner Charter):

   ```yaml
   ---
   title: <Titel>
   date: YYYY-MM-DD
   author: <Agentenname>
   issue: <Paperclip-Issue-ID oder ->
   status: draft | in_review | final
   ---
   ```

3. Committe mit aussagekräftiger Nachricht, z. B. `research: <thema>`.
4. `git push origin main`.

## Git-Authentifizierung

Die Authentifizierung läuft automatisch über den zur Laufzeit injizierten **`GITHUB_TOKEN`** (ein Credential-Helper ist auf dem Host eingerichtet). Du musst **keinen** Token eintragen und **niemals** einen Token-Wert in eine Datei, einen Commit oder einen Kommentar schreiben.

Wenn ein Push fehlschlägt (Auth/Netz): Ergebnis trotzdem lokal committen, das Issue in Paperclip auf `blocked` setzen mit **Owner + konkreter Aktion**. Nichts erfinden, keine Historie löschen, keine `--force`-Pushes.

## Struktur

- `research/` — alle Rechercheergebnisse, ein Dokument pro Thema/Issue.
- `README.md` — Kurzbeschreibung des Repos.
