# Roadmap

- [x] Verify all 15 local originals against hosted storage (SHA-256 identical), embedded model dependencies, and Earth/Moon/Mars locally; no Canvas or asset request errors.
- [x] Add export regression checks (8 tests passing) and stage a complete portable source ZIP including public/assets; Windows execution remains unverified.

- [x] Replace logo and favicon; apply logo palette and lunar/Mars mission themes (Mars palette chosen because uploaded brief ends during lunar section).
- [x] Audit planetary shapes and add shared spherical Earth, Moon, Mars and Sun views across pages; retain intentional local colony terrain.
- [x] Add contextual astronaut inspection animations on the existing Quaternius skeleton without changing mission rules; authored poses, not professional motion clips.
- [x] Verify planet rendering, navigation, construction, walking state and desktop/mobile layout; six tests pass.

- [x] Visual upgrade: NASA-hosted astronaut resource, textured celestial bodies, PBR terrain, engineered facilities, filtered shadows, quality options. This is not AAA photorealism or hardware ray tracing; the available astronaut lacks high-resolution modern suit detail.
- [x] Verify Moon/Mars rendering, selection, construction and existing mission tests.

- [x] Immersive environment upgrade (from uploaded spec):
  - [x] Install three.js / React Three Fiber for React 19
  - [x] 3D lunar + martian terrains (craters, stars, Earth / dusty sky, dunes, mesas)
  - [x] Astronaut character in scene (CC0 Quaternius model, idle bob)
  - [x] Structures appear on terrain when built (solar, oxygen, water, greenhouse, mine, shield) + landing pad
  - [x] Hover/tap tooltips with name, purpose, science fact
  - [x] Camera zoom/pan/orbit, appear animations, hover highlight ring
  - [x] Existing sim logic, missions, briefing intact (all tests pass)
  - [x] Verified in sandbox browser (screenshots, no page errors)

Open (needs the user, not blocking):
- Check smoothness on a real laptop/phone — sandbox renders on CPU, so frame rate and feel couldn't be judged here.
- A fully photorealistic modern EMU needs a professionally licensed high-detail model; the available NASA resource is older and its third-party redistribution rights need confirmation before commercial use.
