# virtmon

`virtmon` is a script for splitting a physical monitor into virtual ones.

![virtmon](https://github.com/nixxxon/virtmon/assets/8500894/25dc518e-8c32-4cb8-ba79-95d6b02d5c29)

One use case is to make screen sharing better (for the viewer) by splitting a large (ultrawide) monitor into smaller ones that can be shared individually.

## Dependencies

- [xrandr](https://www.x.org/wiki/Projects/XRandR)

All dependencies can be installed with your package manager.

## Installation

Download the script, make it executable and add it to your `$PATH`.

```
wget https://raw.githubusercontent.com/nixxxon/virtmon/master/virtmon -q \
    && chmod +x virtmon \
    && sudo mv virtmon /usr/local/bin/virtmon
```

## Usage

Run `virtmon` to split the primary monitor into two equal sized virtual monitors.

```
+-------------+-------------+
|             |             |
|             |             |
|             |             |
|             |             |
+-------------+-------------+
```

Run `virtmon 25,75` to split the primary monitor at 25% and 75% (from the left) resulting in three virtual monitors, 25%, 50% and 25% wide.

```
+------+-------------+------+
|      |             |      |
|      |             |      |
|      |             |      |
|      |             |      |
+------+-------------+------+
```
