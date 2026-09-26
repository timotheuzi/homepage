# ⚔️ BATTLE CHESS

A visceral, cartoon-style chess game built with **Flutter** and the **Flame engine**. Featuring chunky pieces with big personalities and high-impact combat animations.

## Features

- **Unique Fatalities:** Every piece type has a unique, violent death animation—pawns get squashed, rooks crumble, and kings suffer a dramatic shake and fade.
- **Top-Tier Cartoon Animations:** 
  - **Move hop:** pieces anticipate jumps with a squash, hop along an arc, stretch in mid-air, and settle with a bounce.
  - **Fight snap:** captures trigger a wind-up, a snap-lunge attack, screen shake on impact, and a slow retract.
  - **Idle breathing:** pieces gently bob and pulse while waiting.
- **Learning AI**: Features a SQLite-backed neural-inspired learning system. The AI remembers your moves, adopts winning human tactics, and learns to avoid tricks it has fallen for in the past.
- **Dynamic Personalities:** Play against dorky AI personalities like *Sir SnoodleBottom* with varying styles (Position-focused, Aggressive, Tactical).
- **Battle Log & Adaptive Chat:** A real-time log of every move with interactive trash-talking AI that recognizes "tricks" it has seen before.
- **Local Network Multiplayer:** Host or join games over Wi-Fi/LAN for cross-platform head-to-head battles.
- **Snazzy Vector Graphics:** Custom vector pieces drawn entirely with Canvas—chunky outlines, googly eyes, and glossy highlights.
- **Full Chess Rules:** legal move generation, castling, en passant, promotion, and checkmate detection.

## Project layout

```
lib/
  main.dart                  # Flutter app shell & Material UI
  game/
    chess_engine.dart        # Rules engine (Pure Dart)
    chess_ai.dart            # Minimax AI with persistent learning
    learning_database.dart   # SQLite storage for move weights and experience
    multiplayer_manager.dart # Local P2P socket communication
    piece.dart               # Piece model & color definitions
    piece_sprites.dart       # Custom cartoon vector painters
    piece_component.dart     # Flame components with unique fatalities
    board_game.dart          # FlameGame logic, particles, and shake
    game_icon.dart           # Reusable vector app icon widget
```

## License

**Proprietary License**

© 2026 **Dark Work** & **timotheuzi@hotmail.com**. All rights reserved.
Created and owned by **Dark Work**. Unauthorized copying, modification, or distribution of this software is strictly prohibited.
