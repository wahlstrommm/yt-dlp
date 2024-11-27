# yt-dlp

## yt-dlp kommando

### Ladda ner en video

```bash
yt-dlp URL
```

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

