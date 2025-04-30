# Hexamatch

Fractions Brain training excercise by Naadir.

HexaMatch is a browser-based mini-game designed to help beginners build intuition for fractions by clicking hexagon tiles whose values sum to a target fraction or percentage before time runs out.

## Gameplay

1. **Target**  
   A target value (for example, `1`, `1 ½`, or `75%`) appears at the top center of the screen.

2. **Tiles**  
   Hexagon tiles labeled with fractions appear in random positions.

3. **Timer**  
   You have 30 seconds to click (select) tiles whose values add exactly to the target.

4. **Selection**  
   - Click a tile to select it (it turns green).  
   - Click it again to un-select.  
   - If your running sum exceeds the target or the timer reaches zero, you lose a life and the round resets.  
   - If you match the target exactly, you earn points and advance to the next level.

5. **Lives & Score**  
   You start with three lives. Each correct round awards 10 points.

## Quick Start

1. Clone or download this repository.  
2. Open `index.html` in any modern browser (no build step is required).

## Configuration

Near the top of the `<script>` block in `index.html` you will find a `CONFIG` object. You can tweak gameplay parameters there:

```js
const CONFIG = {
  ROUND_TIME: 30,           // seconds per round
  TILE_COUNT: 8,            // number of hexagon tiles each round
  TILE_RADIUS: 44,          // radius in pixels of each tile
  FONT_TILE: '22px Manrope',// font for tile labels
  FONT_HUD: '22px Manrope'  // font for target/current/timer
};
