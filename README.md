# Logo-Inspired Website

use the attached logo for the app and use the color from the logo for the color scheme of website

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/4b609f21-7a75-49f2-86eb-b0c96de04f9b).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Use Node.js 22.12+ (or a newer supported LTS) and npm. On Windows, extract the complete portable ZIP, open that folder in VS Code, and use its terminal:

```sh
npm install
npm run dev
```

Open the local URL printed by Vite. No Lovable asset server or credentials are needed for the textures, logos or models.

### Original assets must be included

Keep the entire `public/assets/` folder when copying or downloading the source. It contains both AstroQuest logos, eleven original planetary/terrain images, and two original GLB files. The GLBs include their own images and buffers; the scene uses the decoded GLB without remote decoders. Files in `src/assets/` ending in `.asset.json` are retained provenance metadata, **not** image files and not runtime imports.

Run `npm run assets:check` to check all original files against their recorded byte sizes, model dependencies and source references. This check also runs before `npm run dev` and `npm run build`; missing files produce a specific filename instead of a Canvas loading crash. If a source export omits binaries, use the complete portable ZIP rather than that incomplete export. Do not replace the original images with generic textures.

`npm test` runs regression tests. `npm run build` creates the production output. Source and license credits are in `src/assets/CREDITS.md`.
