# CRITICAL RULE: FEATURE-FIRST CLEAN ARCHITECTURE (FFCA)
This project strictly enforces FFCA to prevent horizontal monoliths.

1. DIRECTORY STRUCTURE: The root of `lib/` must only contain `core/` and `features/`.
2. VERTICAL SLICING: Every distinct capability (e.g., `reader`, `lore_companion`, `library`) must live inside its own folder within `lib/features/`.
3. INTERNAL LAYERS: Inside every feature folder, you must strictly implement standard Clean Architecture: `data/`, `domain/`, and `presentation/`.
4. DEPENDENCY RULE: `presentation` depends on `domain`. `data` depends on `domain`.
5. FEATURE ISOLATION: A feature's `presentation` layer may consume another feature's Riverpod provider, but it MUST NEVER directly import another feature's `data` layer.
6. NO UI IN DOMAIN: The `domain` and `data` layers must never import `package:flutter/material.dart`. They are pure Dart.
