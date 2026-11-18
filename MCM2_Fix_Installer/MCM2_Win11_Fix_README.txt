MOTOCROSS MADNESS 2 - Windows 10/11 Fix Pack
==============================================

[CZ]
Co balíček dělá:
  * dgVoodoo 2.87.5 (DirectDraw/Direct3D wrapper) - hra běží přes DirectX 12,
    žádné pády v DDraw.dll, nativní rozlišení monitoru (i 16:9 / 1440p / 4K),
    vyhlazování hran 4x, anizotropní filtrování 16x, VSync, bez vodoznaku.
  * Zaregistruje video kodek Intel Indeo 5 (ir50_32.dll) - bez něj hra padá
    v hlavním menu při přehrávání UI\EVENTS.AVI.
  * Doplní d3drm.dll, která ve Windows 10/11 chybí (vlastní minimální náhrada,
    zdrojový kód je přiložen jako d3drm_source.c).
  * Vypne případný režim kompatibility nastavený na MCM2.EXE.
  * Původní soubory zazálohuje do složky MCM2Fix_backup a odinstalace je vrátí.

Použití:
  1. Hru musíš mít nainstalovanou a spustitelnou (balíček neobsahuje hru).
  2. Spusť MCM2_Win11_Fix_Setup.exe, vyber složku hry, Instalovat.
  3. Při prvním spuštění se hra zeptá na 3D kartu - vyber "dgVoodoo DX API Layer".
  4. V Options -> Graphics vyber rozlišení svého monitoru.

Nastavení grafiky lze měnit přes dgVoodooCpl.exe ve složce hry.
Pokud hra po instalaci padá, zkus v dgVoodooCpl změnit Output API na
"Best available" nebo vypnout Antialiasing.

[EN]
What it does:
  * dgVoodoo 2.87.5 wrapper (DirectX 12 output, native/widescreen resolutions,
    4x MSAA, 16x anisotropic filtering, VSync, no watermark).
  * Registers the Intel Indeo 5 codec (fixes the crash in the main menu).
  * Adds a minimal d3drm.dll replacement (missing on Windows 10/11; source included).
  * Removes compatibility-mode flags from MCM2.EXE.
  * Backs up replaced files to MCM2Fix_backup; the uninstaller restores them.

Usage: install the game first, run the setup, select the game folder.
On first launch choose "dgVoodoo DX API Layer" as the 3D card, then pick
your monitor resolution in Options -> Graphics.

Credits:
  dgVoodoo 2 (c) Dege - http://dege.freeweb.hu/ / https://github.com/dege-diosg/dgVoodoo2
  Intel Indeo Video 5 codec (c) Intel Corp.
  The game files are not included.
