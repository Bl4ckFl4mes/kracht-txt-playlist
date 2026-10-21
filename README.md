# TXT → Playlist (Kracht)

**Erstellt automatisch eine Playlist aus einer TXT-Liederliste** — "Künstler - Titel" pro Zeile.

Basiert auf TXT→Queue von EvgenchikS (MIT) — derivative work, MIT License.

## TXT-Format

```
Radiohead — No Surprises
Daft Punk - Get Lucky
1. Queen — Bohemian Rhapsody   (Nummerierung wird automatisch entfernt)
Linkin Park - Numb
```

- Ein Lied pro Zeile, **Trennung "Künstler - Titel"** mit Bindestrich/Gedankenstrich
- Nur Titel geht auch (Match wird schlechter)
- Nummerierung (`1.` `1)`) wird entfernt, `#`-Kommentar-Zeilen ignoriert
- Max 1000 Songs pro Import, 2 MB Datei

## Workflow

1. **Sources → TXT → Playlist** (Widget erscheint im Sources-Tab)
2. TXT-Datei auswählen ODER Liste ins Textfeld einfügen
3. **Mode: Playlist** (Dropdown) + **Playlist-Name** eingeben
4. **Find songs** → sucht jeden Song via aktivem Metadata-Provider (Spotify/SoundCloud/YouTube)
5. Matches prüfen (Auto-Match = exakt, Approx = manuell wählen)
6. **Create playlist** → Playlist wird erstellt mit allen gematchten Songs

## Voraussetzung

Ein Metadata-Provider mit Track-Search (z.B. das Spotify-Plugin) + ein Streaming-Provider (YouTube/Bandcamp/SoundCloud) müssen installiert sein.

## Credits

Fork von [EvgenchikS2/Nuclear_Player_txt_queue](https://github.com/EvgenchikS2/Nuclear_Player_txt_queue) (MIT) — geändert auf Playlists-API statt Queue.
