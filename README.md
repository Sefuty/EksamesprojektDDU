# Skrald Detektering med YOLOv8

Dette projekt implementerer en webbaseret løsning til detektering af forskellige typer skrald ved hjælp af YOLOv8 og ONNX Runtime.

## Funktioner

- Upload billeder direkte i browseren
- Detektering af 18 forskellige typer skrald:
  - Aluminium folie
  - Flaske prop
  - Flaske
  - Knust glas
  - Dåse
  - Karton
  - Cigaret
  - Kop
  - Låg
  - Andet affald
  - Andet plast
  - Papir
  - Plastikpose - indpakning
  - Plastik beholder
  - Dåseprop
  - Sugerør
  - Polystyren stykke
  - Umarkeret affald
- Realtids visning af detekterede objekter med bounding boxes
- Automatisk størrelsesjustering af billeder

## Installation

1. Sørg for at du har følgende filer i din projektmappe:
   - `index.html`
   - `best.onnx` (din trænede YOLOv8 model)

2. Åbn `index.html` i en moderne webbrowser

## Brug

1. Klik på "Vælg fil" knappen for at uploade et billede
2. Vent mens modellen analyserer billedet
3. De detekterede objekter vil blive vist med grønne kasser og labels

## Tekniske Detaljer

- Bruger ONNX Runtime Web til at køre YOLOv8 modellen direkte i browseren
- Understøtter WASM for optimal ydeevne
- Automatisk billedbehandling og størrelsesjustering
- Implementerer Non-Maximum Suppression (NMS) for at undgå overlappende detektioner

## Krav

- En moderne webbrowser med JavaScript aktiveret
- ONNX Runtime Web support
- WASM support i browseren

## Bemærk

Dette projekt er designet til at hjælpe med at identificere og kategorisere forskellige typer affald i billeder, hvilket kan være nyttigt for miljøovervågning og affaldshåndtering. 
