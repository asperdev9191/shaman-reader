# CRITICAL RULE: FLUTTER UI STANDARDS
1. STATELESS DEFAULT: All widgets must be `ConsumerWidget` or `HookConsumerWidget` (from Riverpod). 
2. NO STATEFUL WIDGETS: Do not use `StatefulWidget` unless implementing a highly localized `AnimationController`.
3. BUSINESS LOGIC BAN: Widgets must never contain business logic (no `if` statements calculating lore or spoilers). Widgets only consume and display data from Riverpod Providers.
