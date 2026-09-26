# ⚔️ BATTLE CHESS

A visceral, cartoon-style chess game built with **Flutter** and the **Flame engine**. Featuring chunky 3D-shaded vector pieces with big personalities, vibrant themes, and high-impact combat animations.

## Features

- **Gorgeous Visuals & Themes:**
  - **Board Themes:** Switch seamlessly between **Mahogany Wood**, **Imperial Marble**, **Neon Cyber**, and **Midnight Star** themes.
  - **Tactile 3D Board:** Rendered with tile bevels, inner shadows, theme-matched outer frames, and gold/metallic corner studs.
  - **Polished 3D-Shaded Vector Pieces:** Custom vector pieces painted with radial and linear gradients, specular highlights, glossy sheen, pedestals, and drop shadows.
  - **Last Move & Target Highlights:** Soft glowing trails on previous moves, pulsating selection glow, target lock reticles for captures, and glowing movement rings.
- **High-Impact FX & Fatalities:**
  - **Shockwave Rings & Comic Hit Text:** Captures unleash expanding shockwaves and animated floating text ("BOOM!", "SPLAT!", "FATALITY!", "CRUSH!", "KO!").
  - **Dust Puffs & Check Auras:** Landing dust particles when pieces hop, and a pulsating radial plasma check aura under kings in check.
  - **Unique Fatalities:** Every piece type has a unique death animation—pawns get squashed, rooks crumble, and queens explode into shards.
- **Captured Pieces Tray & Score Bar:** Real-time visual tray displaying captured white and black pieces with live material advantage tracking.
- **Learning AI**: Features a SQLite-backed neural-inspired learning system. The AI remembers your moves, adopts winning human tactics, and learns to avoid tricks it has fallen for in the past.
- **Dynamic Personalities:** Play against dorky AI personalities like *Dr. Snoodlebottom* with varying styles (Position-focused, Aggressive, Tactical).
- **Battle Log & Adaptive Chat:** Real-time log of every move with interactive trash-talking AI that recognizes "tricks" it has seen before.
- **Multiplayer Options:**
  - **Local Network (Wi-Fi):** Host or join games over Wi-Fi/LAN for cross-platform head-to-head battles.
  - **Nearby Play (Bluetooth):** Head-to-head play over Bluetooth without Wi-Fi network required (via `nearby_connections`).
- **Full Chess Rules:** Legal move generation, castling, en passant, promotion, and checkmate detection.

## Project Layout

```
lib/
  main.dart                  # Flutter app shell, Material UI, theme switcher & captured tray
  game/
    board_game.dart          # FlameGame logic, rendering, highlights, and screen shake
    board_theme.dart         # Board themes definitions (Wood, Marble, Cyber, Midnight)
    fx_components.dart       # Shockwave rings, combat hit text, dust particles & check aura
    chess_engine.dart        # Rules engine (Pure Dart)
    chess_ai.dart            # Minimax AI with persistent learning
    grandmaster_patterns.dart # Classic tactical pattern library for the AI
    learning_database.dart   # SQLite storage for move weights and experience
    multiplayer_manager.dart # Local P2P socket communication
    piece.dart               # Piece model & color definitions
    piece_sprites.dart       # Custom 3D-shaded cartoon vector painters
    piece_component.dart     # Flame components with drop shadows, hop dust & fatalities
    game_icon.dart           # Reusable vector app icon widget
```

## License

**Proprietary License**

© 2026 **Dark Work** & **timotheuzi@hotmail.com**. All rights reserved.
Created and owned by **Dark Work**. Unauthorized copying, modification, or distribution of this software is strictly prohibited.
