# Ikigai Saga

A 3D anime-style adventure game that runs in the browser. Pick a hero, explore an open island of tall grass, forests and coasts, fight monsters, hatch pets and take on the Coral Titan world boss.

## Play

Open `index.html` in Chrome or Edge, or serve the folder:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## Heroes

- **Spark Knight**: sword fighter. Thunder Slam, Whirlwind, Rally.
- **Tidecaller**: water mage who heals. Tide Surge, Frost Nova, Bubble Shield.
- **Ember Archer**: ranged fire archer. Ember Rain (a meteor shower), Fire Burst, Second Wind.

## Your own VRoid hero

Make a character in VRoid Studio (free), choose **Export → Export as VRM**, then in the game open **Wardrobe → Load .vrm file**. Your model replaces the built-in hero, keeps your class weapon, and is animated by the game. It is saved in your browser on that device.

## Controls

WASD or arrow keys to move, or click where you want to go. Drag to turn the camera, mouse wheel to zoom. Keys 1, 2, 3 or Space for skills. Enter to chat.

## Notes

- Built with three.js r147 and @pixiv/three-vrm 1.0.6, loaded from jsDelivr.
- Hosted as a plain web page, the game plays solo. Multiplayer, chat, the shared world boss and the leaderboard use Claude artifact features and only work in the Claude-hosted version.
- Nature props and weapon models are by Kenney (CC0). See `assets/*/License.txt`.

## Deploy on Render

`render.yaml` sets this up as a Render static site: create a new Blueprint on Render and point it at this repository.
