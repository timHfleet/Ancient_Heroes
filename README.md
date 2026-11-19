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

Choose Female or Male when you pick your hero, or switch any time in the Wardrobe. Built-in heroes use one licensed anime VRM, about six to seven heads tall. Each class wears original armor on that skeleton: a cape, pauldrons, a tunic or chest piece, a belt, greaves, and a class weapon. The same body is used for both genders. Pets stay small and round. A VRM you load from the Wardrobe replaces the built-in hero. Idle and walk are posed by the game on the VRM skeleton.

## Your own VRoid hero

Make a character in VRoid Studio (free), choose **Export → Export as VRM**, then in the game open **Wardrobe → Load .vrm file**. Your model replaces the built-in hero, keeps your class weapon, and is animated by the game. It is saved in your browser on that device.

## Controls

WASD or arrow keys to move, or click where you want to go. Drag to turn the camera, mouse wheel to zoom. Keys 1, 2, 3 or Space for skills. Enter to chat.

The blue MP bar tracks your main skill. It fills again as the cooldown ends. HP is the red bar and EXP is the gold bar.

## Notes

- Built with three.js r147 and @pixiv/three-vrm 1.0.6, loaded from jsDelivr. Fonts are Cinzel, Philosopher, Outfit and Nunito from Google Fonts (SIL Open Font License).
- Hosted as a plain web page, the game plays solo. Multiplayer, chat, the shared world boss and the leaderboard use Claude artifact features and only work in the Claude-hosted version.
- Nature props, weapons, and the harbor village (Fantasy Town Kit) are by Kenney (CC0). Rounder trees, bushes, rocks and flowers in `assets/q/` are from Quaternius's Ultimate Nature Pack (CC0). See `assets/*/License.txt`. Grass, the dirt path, sky, class armor, house banners, and effects are original. A few accent trees are still procedural.
- `assets/v/hero.vrm` is pixiv's VRM sample model (c) 2022 pixiv Inc. It is the default hero for every class. Its VRM 1.0 license allows redistribution and modification. See `assets/v/LICENSE.txt`.

## Deploy on Render

`render.yaml` sets this up as a Render static site. The service slug stays `ikigai-saga` so an existing Blueprint deploy and its URL keep working. To show the new title in the Render dashboard, rename the service's display name there. Changing the `name` field in `render.yaml` would provision a different service.
