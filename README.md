# Keepy-Uppy Phone

Keep a ball bouncing on your phone screen. Flick the phone up to launch the ball, follow its shadow, and lift into each landing to keep it going. Faster impacts score more.

**Play:** open https://dcstuff.github.io/keepy-uppy-phone/ on your phone and tap **Play**. The game is motion-only: it needs the phone's accelerometer and gyro, which browsers only share over HTTPS (GitHub Pages provides that). On an iPhone, Safari will ask for motion permission.

- `index.html` is the game, a single self-contained file.
- `game.html` is the same game without the page wrapper, used for the Claude artifact version.

**How to flick:** hold the phone flat, then give it a short, sharp pop upward and stop dead, like tossing a pancake. A slow lift won't launch the ball. The meter at the bottom of the screen shows your upward speed against the launch threshold (red mark), and tells you why a flick didn't count: too gentle, not a sharp enough stop, or the screen tilted more than about 60°.

Tuning settings are at the top of the script: `LAUNCH_GAIN`, `TILT_GAIN`, `CHASE_GAIN`, `SPIN_GAIN` and `E` for the physics, and `FLICK_MIN_V` (upward speed a flick needs, default 0.35 m/s) and `FLICK_BRAKE` (braking that releases the ball, default 2.5 m/s²) in the sensor section.
