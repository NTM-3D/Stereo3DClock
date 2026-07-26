# Stereo 3D Clock

HTML file that renders an animated 3D scene with a floating
digital clock, in stereoscopic 3D. No build step or dependencies — just open the file in a browser.

https://ntm-3d.github.io/Stereo3DClock

## How it works

Each scene is drawn twice per frame — once per eye — onto a shared 3D world,
then composited into the output canvas in the selected 3D format. The clock
floats through the scene and is depth-sorted with the rest of the objects.

## Scenes

- **Deep Space** – a slowly rotating starfield.
- **Neon Grid** – a synthwave sunset over a checkered floor, with glowing
  monoliths.
- **City Skyline** – a night skyline with lit windows, a moon, and passing
  traffic.
- **Snowfall** – falling snow over a dark gradient sky.
- **Bubbles** – rising, swaying bubbles.
- **Star Tunnel** – stars flying past from a central vanishing point.
- **Aurora** – layered aurora ribbons over a ridge silhouette.
- **Desert Dunes** – layered dune silhouettes under a setting sun.
- **Fireflies** – drifting, blinking fireflies over a dark field.
- **The Matrix** – falling glyph columns rendered from a pre-built character
  atlas.

## Output formats

- **Interlaced** – alternating rows for line-interlaced 3D displays.
- **Half TAB** – top-and-bottom, each eye squeezed into half height.
- **Half SBS** – side-by-side, each eye squeezed into half width.
- **WebXR** – side-by-side, each eye squeezed into half width.

A "Swap eyes" option is available if a display's left/right output is reversed.

## Controls

Depth, convergence, and clock text size are adjustable from the menu before
starting, or live during playback. Once the viewer is running, press the
on-screen **?** button (or open the help panel) for the full list of keyboard, remote
and touch controls.

## URL parameters

The viewer can be launched directly with settings pre-filled and playback
started automatically, e.g.:

```
*.html?depth=100&convergence=100&clocksize=100&scene=deepspace&format=interlaced&swap=0&auto=1
```

The help panel's "Copy auto URL" button generates this link for the current
settings.
