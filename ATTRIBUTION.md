# Risk Command — third-party asset attribution

Every imported asset below is released under **CC0 1.0 Universal (public domain)**.
No attribution is legally required, but we credit the sources anyway.
Assets were mesh-decimated with meshoptimizer (via glTF-Transform), their
textures resized to 1024/512/256 px, and draw calls merged (`flatten` + `join`)
so they fit mobile browser budgets. In-game shaders tint the soldiers per
faction and weather the props (desaturation, grime, dust, snow, wet and burnt
looks). The source files are otherwise unmodified.

## Characters — Grab3D (CC0) — https://grab3d.com
- `assets/characters/soldier.glb`: "Soldier" (rigged, walk/run clips),
  https://grab3d.com/models/characters/soldier/
  Decimated from about 279k to about 10k triangles with 1024 px PBR textures. Faction camo comes from `assets/shaders/soldier.gdshader`.
  Idle, aim, fire, reload, crouch, hit and death poses are layered procedurally on the rig (`scripts/battle/soldier_model.gd`).
- `assets/characters/soldier_token.glb`: the same model decimated to about 1.5k triangles with 256 px textures, used for the globe army tokens.

## Environment props — Grab3D (CC0) — https://grab3d.com/models/
apartment-building, bush, cactus, cement-bags, concrete-pipe, dead-tree,
dumpster, fishing-boat, fuel-tank, guard-tower, helicopter, jersey-barrier,
lighthouse, monstera-plant, oak-tree, office-building, palm-tree, pickup-truck,
pine-tree, sandbags, sedan, shipping-container-proz, site-office,
snowy-pine-tree, spiked-barricade, steel-beam-stack, stone-house, street-light,
suv, tractor, traffic-barrel, trash-bag-pile, utility-pole, water-tower,
wooden-pallet, wooden-watchtower (`assets/props/<name>.glb`).

## Photo-scanned props — Poly Haven (CC0) — https://polyhaven.com/models
(`assets/props/ph_<id>.glb`) Barrel_01, barrel_03, wooden_crate_01, wooden_crate_02,
old_military_crate, wooden_military_crate, metal_jerrycan_green,
concrete_road_barrier_02, covered_car, namaqualand_boulder_02,
namaqualand_boulder_05, dead_tree_trunk, tree_stump_01, fern_02, metal_trash_can.

## Ground textures — Poly Haven (CC0) — https://polyhaven.com/textures
(`assets/ground/<id>_albedo.jpg`, 512 px diffuse) aerial_sand, cracked_red_ground,
rock_face_03, asphalt_02, cracked_concrete, rubble, forest_leaves_02, mud_forest,
snow_02, aerial_rocks_02, coast_sand_01, aerial_grass_rock.

## Sky panoramas — Poly Haven HDRIs (CC0) — https://polyhaven.com/hdris
(`assets/sky/*.jpg`, tonemapped 2048x1024 LDR) qwantani_noon_puresky,
kloofendal_48d_partly_cloudy_puresky, kloofendal_overcast_puresky,
snow_field_puresky, kloofendal_28d_misty_puresky.

## Everything else
The globe, terrain, weapons, procedural props, effects, audio and UI are generated in code
by this project.
