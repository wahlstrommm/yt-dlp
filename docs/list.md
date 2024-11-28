---
title: "List"
password: "list_password"
---

# Webbplatser och tjänster som stöds av yt-dlp

# tjänster som stöds av yt-dlp

**yt-dlp** är ett kraftfullt verktyg som stöder nedladdning från en stor mängd webbplatser. Här är en sammanfattning av några populära kategorier och tjänster:

---

## **1. Videoplattformar**
- **YouTube**  
  - Videor, spellistor, kanaler, och "Members Only"-innehåll (med autentisering).
- **Vimeo**
- **Dailymotion**
- **TikTok**
- **Twitch**  
  - Ladda ner klipp, VODs och streams.
- **Facebook** (publikt innehåll)
- **Instagram** (inlägg, Stories, Reels, IGTV)

---

## **2. Musikplattformar**
- **SoundCloud**  
  - Individuella spår och spellistor.
- **Bandcamp**  
  - Album och enskilda låtar.
- **Mixcloud**  
  - DJ-set och mixar.
- **Audiomack**

---

## **3. Sociala medier**
- **Reddit**  
  - Ladda ner inbäddade videor och gifs.
- **Twitter (X)**  
  - Ladda ner inbäddade videor och media från tweets.

---

## **4. Streamingplattformar**
Med viss autentisering och konfiguration:
- **Netflix** (Kräver M3U8-stöd, endast för utbildningsändamål).
- **Hulu**
- **Amazon Prime Video**
- **Disney+**

⚠️ **Notera:** Streamingtjänster har ofta DRM-skydd, vilket kan kräva avancerade inställningar. Nedladdning kan strida mot deras användarvillkor.

---

## **5. Nyhets- och mediawebbplatser**
- **BBC iPlayer**
- **SVT Play**
- **CNN**
- **The Guardian**

---

## **6. Live-streamar**
- **YouTube Live**
- **Twitch Live**
- **Facebook Live**

Du kan ladda ner live-innehåll under pågående stream eller efter att det avslutats.

---

## **7. Lärandeplattformar**
- **Khan Academy**
- **Udemy** (Kräver inloggning)
- **Coursera** (Kräver inloggning)

---

## **8. Pornografiska plattformar**
- **Pornhub**
- **XVideos**
- **RedTube**

⚠️ Respektera lokala lagar och plattformens användarvillkor.

---

## **9. Fildelning och annan media**
- **Google Drive** (publika filer)
- **Mega.nz** (publika länkar)
- **WeTransfer**

---

## **Hur hittar du alla stödda webbplatser?**

För att se en fullständig lista över alla webbplatser som stöds, kör:
```bash
yt-dlp --list-extractors
```

## Tips om specifika webbplatser

Om en webbplats inte fungerar, kontrollera om den stöds med:
``
yt-dlp --list-extractors
``

Uppdatera yt-dlp för att få senaste stödet:

``
pip install -U yt-dlp
``

Felsök problem med:

``
yt-dlp -v <URL>
``
