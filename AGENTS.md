<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.

## What Lovable manages

Rules outside this block are the project's own. Change the pieces below in
Lovable, not by hand. With the [Lovable MCP](https://mcp.lovable.dev)
connected, `send_message` asks Lovable to do it; otherwise ask the user to
use the editor.

- **Database.** Do not add or edit `supabase/migrations/` or `drizzle/`.
  Ask Lovable to change the schema.
- **Generated files.** Do not edit a file whose header says it is automatically
  generated.
- **AI gateway.** Keep model calls on Lovable's gateway, and keep
  `LOVABLE_API_KEY` out of browser code.
- **Connectors.** Lovable provides native connectors. `list_connectors` shows
  which are enabled; `add_connector` only returns the dashboard link. When a
  connector is enabled, calls go through the connector gateway and need
  `LOVABLE_API_KEY`. When Lovable does not provide one, users can bring their
  own key and store it in Secrets.
- **Secrets.** Lovable manages them. Do not put secret values in the repo.
<!-- LOVABLE:END -->

- Keep visual upgrades in src/scene and preserve src/lib/sim.ts as the independent mission-rule boundary; graphics quality must never affect economics or outcomes.
- Resolve Three.js material colors from semantic --scene-* CSS roles; serve media from public/assets via root-relative paths (no /__l5e URLs) so the app runs locally; keep source/license credits in src/assets/CREDITS.md.
- Keep original binaries in portable source deliveries and run scripts/check-local-assets.mjs before npm dev/build; provenance metadata alone cannot load textures or models in exported projects.
- The planetary Canvas mounts only after hydration; use local environment lighting and decoded GLBs to avoid runtime third-party decoder or HDR dependencies.
- Whole-world views share CelestialBody SphereGeometry via PlanetGallery; playable heightfield terrain remains a local construction site, not a globe representation.
- Keep astronaut inspection motion in scene-only pure helpers with interruptible target state; it must not change simulation rules or construction costs.
