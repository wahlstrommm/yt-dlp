---
title: "yt-dlp Kommando"
password: "yt_dlp_password"
---

# yt-dlp kommando

## Ladda ner en video

```bash
yt-dlp URL
```

### MP4-format med antingen textade eller autogenererade undertexter

```bash
yt-dlp -f mp4 --write-subs --write-auto-sub --sub-lang <språkkod> --convert-subs srt URL
```

#### Förklaring

- ```-f mp4:``` Väljer MP4-format för videon.
- ```--write-subs:``` Laddar ner undertexter om de är tillgängliga.
- ```--write-auto-sub:``` Använder autogenererade undertexter om vanliga inte finns.
- ```--sub-lang <språkkod>:``` Anger språk för undertexterna (t.ex. en för engelska eller sv för svenska).
- ```--convert-subs srt:``` Konverterar undertexterna till SRT-format, som är kompatibelt med många spelare.
- ```URL:``` Byt ut detta mot videons URL.

#### Exempel

Om du vill ladda ner en video med engelska undertexter (vanliga eller autogenererade):

```bash
yt-dlp -f mp4 --write-subs --write-auto-sub --sub-lang en --convert-subs srt https://example.com/video
```

- Om både vanliga och autogenererade undertexter är tillgängliga, laddas de vanliga ner som standard.

- Om du bara vill ha videon med vanliga undertexter och ignorera autogenererade, ta bort ```--write-auto-sub.```

### Ladda ner mp3

```bash
yt-dlp -x --audio-format mp3 URL
```

### Välj högsta kvalitet (video och ljud kombinerat)

```bash
yt-dlp -f best URL
```

### Ange utdatafilens namn

```bash
yt-dlp -o "%(title)s.%(ext)s" URL
```

### Ladda ner spellista (video och ljud)

```bash
yt-dlp --yes-playlist URL
```

### Ladda ner spellista (video och ljud med undertexter)

```bash
yt-dlp --yes-playlist --write-subs --write-auto-sub URL
```

## Soundcloud

### Grundläggande kommando:

```bash
yt-dlp <URL>
```

### Ladda ner som MP3 :

```bash
yt-dlp -x --audio-format mp3 <URL>
```

``
-x
``
: Extraherar ljudet.

``
--audio-format mp3
``
: Konverterar ljudet till MP3-format

### Ladda ner en hel spellista :

```bash
yt-dlp --yes-playlist <URL>
```

### Anpassa filnamn:

Om du vill namnge filerna baserat på titel och artist från SoundCloud:

```bash
yt-dlp -o "%(artist)s - %(title)s.%(ext)s" <URL>
```

Exempelutdata:

``
Artist - Song Title.mp3
``
