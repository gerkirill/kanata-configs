# Kanata Keyboard Mappings

This repository contains keyboard remapping configurations for [Kanata](https://github.com/jtroo/kanata), a keyboard remapper that works on the OS level.

## Getting Started

### Download

Kanata executable can be downloaded from [here](https://github.com/jtroo/kanata/releases) or by using the provided script:

```bash
./download.sh
```

This will download Kanata v1.8.1, make it executable, and display the version.

### Running

The repository includes two different configuration approaches:

1. **Traditional Layer-based** (`layers.kbd`):
   ```bash
   sudo ./kanata -c layers.kbd
   ```

2. **Layer Map with Home Row Mods** (`layermap.kbd`):
   ```bash
   sudo ./kanata -c layermap.kbd
   ```
   
   Or use the provided script:
   ```bash
   ./run.sh
   ```

## Configuration Approaches

### Traditional Layer-based (`layers.kbd`)

This configuration uses the standard `deflayer` approach with a defined source layout and mapped layers.

Features:
- Concurrent tap-hold functionality
- Home row modifiers
- Chords for common actions
- Extra layer for navigation

### Layer Map with Home Row Mods (`layermap.kbd`)

This configuration uses the `deflayermap` approach with more extensive home row mods (HRM) and additional features.

Features:
- Process unmapped keys
- Custom character-modifier templates
- Extended home row modifiers
- Comprehensive extra layer with navigation, brackets, and symbols

## Special Behaviors

### Tap-Hold Keys

| Key         | Tap Function | Hold Function |
|-------------|--------------|---------------|
| `caps`      | Caps Lock    | Left Ctrl     |
| `a`         | a            | Left Meta     |
| `s`         | s            | Left Alt      |
| `d`         | d            | Left Ctrl     |
| `f`         | f            | Left Shift    |
| `j`         | j            | Right Shift   |
| `k`         | k            | Right Ctrl    |
| `l`         | l            | Left Alt      |
| `;`         | ;            | Right Meta    |
| `x`/`.`     | x/.          | Right Alt     |
| `spc`       | Space        | Extra layer   |
| `Right Alt` | Enter        | Right Alt     |
| `Right Ctrl`| Backspace    | Right Ctrl    |

### Chords

| Combination | Function                          |
|-------------|-----------------------------------|
| `w + e`     | Esc (when tapped within 50ms)    |
| `i + o`     | Backspace (when tapped within 50ms) |

## Extra Layer

### Navigation

| Key       | Function                          |
|-----------|-----------------------------------|
| `h`       | Left Arrow                        |
| `j`       | Down Arrow                        |
| `k`       | Up Arrow                          |
| `l`       | Right Arrow                       |
| `n`       | Home                              |
| `m`       | End                               |

### Brackets and Symbols

| Key       | Function                          |
|-----------|-----------------------------------|
| `d`       | (                                 |
| `e`       | )                                 |
| `s`       | [                                 |
| `w`       | ]                                 |
| `f`       | {                                 |
| `r`       | }                                 |
| `1-0`     | !@#$%^&*()                        |
| `-`       | _                                 |
| `=`       | +                                 |

## Customization

To customize these configurations:

1. Edit either `layers.kbd` or `layermap.kbd` based on your preference
2. Refer to the [Kanata Configuration Guide](https://github.com/jtroo/kanata/blob/main/docs/config.adoc) for detailed documentation
3. Run Kanata with your modified configuration

## Force Exit

Press and hold all three keys simultaneously to force exit Kanata:
- Left Control
- Space
- Escape
