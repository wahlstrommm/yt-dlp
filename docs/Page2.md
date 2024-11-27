# Installation

# Steg för steg: Installera yt-dlp

Den här guiden visar hur du installerar **yt-dlp**, ett kraftfullt verktyg för att ladda ner videor och ljud från olika plattformar som YouTube, SoundCloud, och många fler.

---

## **Steg 1: Kontrollera Python-installation**

1. Öppna terminalen (Command Prompt, Terminal eller liknande).
2. Kontrollera att Python är installerat genom att köra:

   ```bash
   python --version
    ```

eller

``
python3 --version
``

### Om Python inte är installerat:

 - Gå till Python.org och ladda ner den senaste versionen.

 - Följ installationsanvisningarna. Se till att markera "Add Python to PATH" under installationen.

## Steg 2: Installera yt-dlp med pip

Använd ``pip`` , Python-pakethanteraren, för att installera yt-dlp. Kör följande kommando:

``
pip install -U yt-dlp
``

Flaggförklaring:

``-U``: Uppdaterar till den senaste versionen om yt-dlp redan är installerat.

Kontrollera att yt-dlp har installerats korrekt genom att köra:

``
yt-dlp --version
``

Om du ser en versionsnummerutskrift är yt-dlp installerat och redo att användas.

## Steg 3: Installera beroenden för ljudkonvertering (FFmpeg)

Varför behövs FFmpeg?

FFmpeg krävs om du vill extrahera ljud, konvertera format eller förbättra prestandan vid nedladdning.

    Ladda ner FFmpeg från FFmpeg.org.

    Följ installationsanvisningarna för ditt operativsystem:

        Windows:
            - Ladda ner en Windows-kompatibel version från Gyan.dev.
            - Extrahera filerna och lägg till FFmpeg i din PATH. Detta görs via:
                - Högerklicka på "Den här datorn" > "Egenskaper".
                - Klicka på "Avancerade systeminställningar" > "Miljövariabler".
                - Under "Systemvariabler", hitta Path, klicka på "Redigera", och lägg till sökvägen till din FFmpeg-mapp (t.ex. C:\ffmpeg\bin).
  
Verifiera att FFmpeg är korrekt installerat:

``
ffmpeg -version
``