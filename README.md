# i3blocks-stop-watch

A simple stopwatch timer for i3blocks

# Usage

Start/stop the stopwatch by left-clicking on the block.

Reset it by right-clicking on the block.

### Installing

```
sudo cp stopwatch /usr/bin
```

- Add the following to the i3blocks.conf:

```
# Stopwatch
[stopwatch]
label=⏱
interval=1
command=stopwatch
```

- If desired keybindings can be added to i3 to control the stopwatch, for example:

```
# Start/Stop stopwatch
bindsym Pause exec env BLOCK_BUTTON=1 stopwatch
# Reset stopwatch
bindsym Shift+Pause exec env BLOCK_BUTTON=3 stopwatch
```
