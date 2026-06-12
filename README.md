# Tomb Raider (2013) Keyboard and Mouse fix

## How-to
1. Open the executable in a hex-editor
2. Disable Auto-Rotating Camera
- horizontal
  - Search for "08 B0 01 D9 9E A0 0F 00 00" and replace it with "08 B0 01 90 90 90 90 90 90"
- vertical
  - Search for "D9 5E 04 D9 44 24 0C D9 5E 0C D9 44 24 18 D9 5E 10 C6 87 C4 0F 00 00 01 E9 A2 FE FF FF DD D8 6A 00 D9 87 40 06 00 00 83 EC 0C D9 5C 24" and replace it with "D9 5E 20 D9 44 24 0C D9 5E 0C D9 44 24 18 D9 5E 10 C6 87 C4 0F 00 00 01 E9 A2 FE FF FF DD D8 6A 00 D9 87 40 06 00 00 83 EC 0C D9 5C 24"
3. Disable Camera Shake while walking
- Search for "8B CF ?? ?? ?? ?? ?? 84 C0 74 ?? 56" and replace it with "8B CF ?? ?? ?? ?? ?? 84 C0 EB ?? 56"
- or change byte 0099b97 to "EB"

## Sources
- https://www.nexusmods.com/tombraider2013/mods/90
- https://www.nexusmods.com/tombraider2013/mods/91
