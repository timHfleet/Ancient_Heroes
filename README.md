# Ancient Heroes

A bright anime-fantasy adventure that runs in the browser. Pick a hero, explore an open island of meadows, forests and coasts, fight monsters, hatch pets and take on the Coral Titan world boss.

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

## Female or male

Choose Female or Male when you pick your hero, or switch any time in the Wardrobe. The female hero is a licensed anime VRM, about six to seven heads tall; the male hero, Kiri, is a VRoid model at `assets/v/hero-male.vrm` (if that file is missing, male heroes use the female body with a broader build). Each class recolours the model's own hair and clothes and holds its class weapon in the fist. Pets stay small and round. A VRM you load from the Wardrobe replaces the built-in hero. Idle and walk are posed by the game on the VRM skeleton.

## Hair and clothes colours

In the Wardrobe, pick a hair colour, a top colour and a bottoms colour. The striped swatch goes back to the class colours. Your choice is saved in your browser and other players see it.

## Your own VRoid hero

Make a character in VRoid Studio (free), choose **Export → Export as VRM**, then in the game open **Wardrobe → Load .vrm file**. Your model replaces the built-in hero, keeps your class weapon, and is animated by the game. It is saved in your browser on that device.

## Controls

WASD, the arrow keys, or the on-screen joystick to move. Click where you want to go. Drag to turn the camera, mouse wheel to zoom. The skill wheel holds the basic attack, three skills (keys 1, 2, 3 or Space), auto hunt, and a dodge. Enter to chat. A line starting with `/recruit` is tagged as a recruit message.

The round portrait shows your level, name, and power. The slim green bar is health. Skill buttons sweep a cooldown. Yellow and orange numbers are damage you deal, green is healing, and red is damage you take.

## Notes

- Built with three.js r147 and @pixiv/three-vrm 1.0.6, loaded from jsDelivr. Fonts are Cinzel, Philosopher, Outfit and Nunito from Google Fonts (SIL Open Font License).
- Hosted as a plain web page, the game plays solo. Multiplayer, chat, the shared world boss and the leaderboard use Claude artifact features and only work in the Claude-hosted version.
- Nature props, weapons, and the harbor village (Fantasy Town Kit) are by Kenney (CC0). Rounder trees, bushes, rocks and flowers in `assets/q/` are from Quaternius's Ultimate Nature Pack (CC0). See `assets/*/License.txt`. Grass, the dirt path, sky, monsters, house banners, and effects are original. A few accent trees are still procedural.
- `assets/v/hero.vrm` is pixiv's VRM sample model (c) 2022 pixiv Inc. It is the default hero for every class. Its VRM 1.0 license allows redistribution and modification. See `assets/v/LICENSE.txt`.

## Deploy on Render

`render.yaml` sets this up as a Render static site. The service slug stays `ikigai-saga` so an existing Blueprint deploy and its URL keep working. To show the new title in the Render dashboard, rename the service's display name there. Changing the `name` field in `render.yaml` would provision a different service.
