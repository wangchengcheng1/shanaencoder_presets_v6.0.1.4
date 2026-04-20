# Mission Cards

## Size Rush

- Goal: reduce size as much as possible.
- Allowed changes: increase CRF, tighten qmin, optional lower audio bitrate.
- Fail condition: obvious blocking in dark scenes.

## Quality Keeper

- Goal: preserve detail in skin/motion/dark scenes.
- Allowed changes: lower CRF, tighten qmax.
- Fail condition: size explosion beyond storage budget.

## Speed Run

- Goal: shorten encode time.
- Allowed changes: faster preset, lighter filter chain.
- Fail condition: visible quality collapse.

## SameAudio Saver

- Goal: keep source audio untouched.
- Allowed changes: `-c:a copy`, video-side tuning only.
- Fail condition: source audio incompatible with target container.
