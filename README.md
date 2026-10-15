# 2 Blind Mice

A local co-op puzzle game prototype. You (and maybe a friend) are tiny mice on a giant mechanical keyboard. Jump on the keys to type out an email on the monitor, then jump on Enter to send it.

Built with Three.js / WebGL in a single HTML file. There's no build step.

## Play

Open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8765
```

Then go to http://localhost:8765.

## Controls

| Player | Move | Jump |
| --- | --- | --- |
| P1 | W A S D | Space |
| P2 (press an arrow to join) | Arrow keys | Enter / Right Shift |

`R` resets the current draft and `M` mutes the sound.

## How it works

- Landing on a key after a jump or fall presses it and types its character. Walking across keys doesn't type.
- Wrong letters show in red. Backspace deletes one, and Esc clears the whole draft.
- Shift stays held while a mouse stands on it, so one player holds Shift while the other types capitals. Solo players can use Caps Lock.
- Mice can stand on each other's heads to jump higher.

## Levels

1. `hi`: tutorial
2. `need cheese`: spacebar and typos
3. `top`: raised keys and a ruler to climb (parkour)
4. `Boss, I QUIT.`: capitals with Shift or Caps Lock
