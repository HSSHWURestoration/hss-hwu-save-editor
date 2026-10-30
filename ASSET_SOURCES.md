# Save Editor Game Art Provenance

These are direct copies from the named original game asset folders. The originals were read only; these copies are bundled with the publicly hosted editor.

For editor capabilities, deployment, privacy, and validation limitations, see [README.md](README.md). Backup-based validation is limited to the exact checks documented below; it does not imply exhaustive field coverage or validation in either game.

| Game | Source | Sandbox copy | Format / dimensions | Use |
|---|---|---|---|---|
| HSS | `HighSchoolStoryRestoredv1.apk/assets/loading_screen.png` | `assets\hss\loading_screen.png` | PNG, 568×360 | Masthead and softened page backdrop |
| HSS | `HighSchoolStoryRestoredv1.apk/assets/banner_background.png` | `assets\hss\banner_background.png` | PNG, 462×53 | Section-heading background |
| HWU | `HollywoodURestoredv1.apk/assets/loading_screen.png` | `assets\hwu\loading_screen.png` | PNG, 568×360 | Masthead and softened page backdrop |
| HWU | `HollywoodURestoredv1.apk/assets/banner_background.png` | `assets\hwu\banner_background.png` | PNG, 462×53 | Section-heading background |

## Native interface assets

The interface assets below are direct copies from each game's original asset folder. They are used as CSS border-image/background-image sources for panels, controls, buttons, badges, and headings. The `-hd` PNGs are kept at their original resolution; the browser scales them for the editor layout. `Display.ttf` is a sandbox-local filename for the game's own title font.

| Game | Source | Sandbox copy | Format / dimensions | Use |
|---|---|---|---|---|
| HSS | `assets\popup-hd.png` | `assets\hss\ui\panel.png` | PNG, 126×126 | Nine-slice cards, dialogs, and text-entry surfaces |
| HSS | `assets\dialog_background-hd.png` | `assets\hss\ui\control.png` | PNG, 48×48 | File drop area, overview tiles, and footer surface |
| HSS | `assets\tab_closet-hd.png` | `assets\hss\ui\button.png` | PNG, 72×44 | Default button state |
| HSS | `assets\tab_closet_selected-hd.png` | `assets\hss\ui\button_selected.png` | PNG, 72×44 | Primary/selected button state |
| HSS | `assets\Freshman.ttf` | `assets\hss\ui\Display.ttf` | TrueType font | Editor title display type |
| HSS | `assets\OpenSans-CondBold.ttf` | `assets\hss\ui\OpenSans-CondBold.ttf` | TrueType font | Game UI text |
| HSS | `assets\OpenSans-ExtraBold.ttf` | `assets\hss\ui\OpenSans-ExtraBold.ttf` | TrueType font | Emphasized game UI text |
| HWU | `assets\popup-hd.png` | `assets\hwu\ui\panel.png` | PNG, 126×126 | Nine-slice cards, dialogs, and text-entry surfaces |
| HWU | `assets\dialog_background-hd.png` | `assets\hwu\ui\control.png` | PNG, 48×48 | File drop area, overview tiles, and footer surface |
| HWU | `assets\tab_closet-hd.png` | `assets\hwu\ui\button.png` | PNG, 200×44 | Default button state |
| HWU | `assets\tab_closet_selected-hd.png` | `assets\hwu\ui\button_selected.png` | PNG, 200×44 | Primary/selected button state |
| HWU | `assets\LobsterTwo-BoldItalic.ttf` | `assets\hwu\ui\Display.ttf` | TrueType font | Editor title display type |
| HWU | `assets\OpenSans-CondBold.ttf` | `assets\hwu\ui\OpenSans-CondBold.ttf` | TrueType font | Game UI text |
| HWU | `assets\OpenSans-ExtraBold.ttf` | `assets\hwu\ui\OpenSans-ExtraBold.ttf` | TrueType font | Emphasized game UI text |
| HSS | `assets\interface-hd.png` atlas frame `banner_name.png` | `assets\hss\ui\section_banner.png` | PNG, 212×24; not rotated | Section-heading ribbon |
| HWU | `assets\interface-hd.png` atlas frame `banner_name.png` | `assets\hwu\ui\section_banner.png` | PNG, 212×24; rotated in atlas and restored on extraction | Section-heading ribbon |
| HSS | `assets\interface-hd.png` atlas frame `button_HUD_plus.png` | `assets\hss\ui\icons\button_HUD_plus.png` | PNG, 46×48; rotated in atlas and restored on extraction | Collapsed Full save data indicator |
| HSS | `assets\interface-hd.png` atlas frame `button_hide.png` | `assets\hss\ui\icons\button_hide.png` | PNG, 60×64; not rotated; visible minus symbol | Expanded Full save data indicator |
| HSS | `assets\interface-hd.png` atlas frame `button_done.png` | `assets\hss\ui\icons\button_done.png` | PNG, 100×104; rotated in atlas and restored on extraction | Download edited save action |
| HSS | `assets\interface-hd.png` atlas frame `button_cancel.png` | `assets\hss\ui\icons\button_cancel.png` | PNG, 100×104; rotated in atlas and restored on extraction | Revert all and cancel-selection actions |
| HWU | `assets\interface-hd.png` atlas frame `button_done.png` | `assets\hwu\ui\icons\button_done.png` | PNG, 100×102; not rotated | Download edited save action |
| HWU | `assets\interface-hd.png` atlas frame `button_cancel.png` | `assets\hwu\ui\icons\button_cancel.png` | PNG, 100×102; not rotated | Revert all and cancel-selection actions |
| HSS | `assets\gamemaker_thumbnails-hd.png` atlas frames `*-thumb.png` | `assets\hss\ui\portraits\` | 68 named PNG crops; atlas is 1024×1024 | Exact-original-name classmate portraits |
| HWU | `assets\gamemaker_thumbnails-hd.png` atlas frames `*-thumb.png` | `assets\hwu\ui\portraits\` | 93 named PNG crops; atlas is 1024×1024 | Exact-original-name classmate portraits |
| HWU | `assets\interface-hd.png` atlas frame `button_HUD_plus.png` | `assets\hwu\ui\icons\button_HUD_plus.png` | PNG, 46×48; rotated in atlas and restored on extraction | Collapsed Full save data indicator |
| HWU | `assets\interface-hd.png` atlas frame `button_hide.png` | `assets\hwu\ui\icons\button_hide.png` | PNG, 60×62; not rotated; visible minus symbol | Expanded Full save data indicator |

The browser HWU profile is based on an existing read-only HWU save-format reference implementation; this is provenance for parsing behavior, not a copied asset.

## HUD sprite icons

The icons below are pixel crops of the named frames in each game's 2048×2048 `assets\interface-hd.png` atlas. Their atlas coordinates and rotation flags were read from `assets\interface-hd.plist`; rotated frames are cropped using the swapped frame dimensions so adjacent atlas pixels are not included. The game-side `assets\HUD.ccb` maps these frame names to the HUD meter nodes. The editor uses the verified icons next to the corresponding quick-field and overview labels.

| Game | Source atlas frame | HUD layout evidence | Sandbox copy | Extracted dimensions |
|---|---|---|---|---|
| HSS | `icon_HUD_coin.png` | `HUD.ccb`: `coinsIcon@` | `assets\hss\ui\icons\icon_HUD_coin.png` | PNG, 48×50 |
| HSS | `icon_HUD_ring.png` | `HUD.ccb`: `heartsIcon@` | `assets\hss\ui\icons\icon_HUD_ring.png` | PNG, 62×46 |
| HSS | `icon_HUD_book.png` | `HUD.ccb`: `starsIcon@` | `assets\hss\ui\icons\icon_HUD_book.png` | PNG, 76×48 |
| HSS | `icon_HUD_pencil.png` | `HUD.ccb`: `pencilIconSprite@` | `assets\hss\ui\icons\icon_HUD_pencil.png` | PNG, 50×48 |
| HSS | `icon_HUD_ticket.png` | `HUD.ccb`: `ticketIconSprite@` | `assets\hss\ui\icons\icon_HUD_ticket.png` | PNG, 70×50 |
| HSS | `icon_coin_small.png` | `store_item_currency.ccb`: `costIconSprite@`, `currencyItemIconSprite@` | `assets\hss\ui\icons\icon_coin_small.png` | PNG, 30×30; documented store icon, not currently displayed |
| HWU | `icon_HUD_coin.png` | `HUD.ccb`: `coinsIcon@` | `assets\hwu\ui\icons\icon_HUD_coin.png` | PNG, 56×54 |
| HWU | `icon_HUD_ring.png` | `HUD.ccb`: `heartsIcon@` | `assets\hwu\ui\icons\icon_HUD_ring.png` | PNG, 56×50 |
| HWU | `icon_HUD_ticket.png` | `HUD.ccb`: `ticketIconSprite@` | `assets\hwu\ui\icons\icon_HUD_ticket.png` | PNG, 70×64 |
| HWU | `icon_coin_small.png` | `store_item_currency.ccb`: `costIconSprite@`, `currencyItemIconSprite@` | `assets\hwu\ui\icons\icon_coin_small.png` | PNG, 36×36; documented store icon, not currently displayed |

The visible editor resource names are based on each game's `assets\strings.json`, not protobuf schema names or sprite filenames: HSS uses XP, Coins, Rings, Books, Pencils, and Tickets; HWU uses XP, Cash, Diamonds, Books, Pencils, and Tickets. The player-field numbers and wire encoding remain unchanged. `HUD.ccb` confirms the relevant HUD-node/frame mappings, but does not establish localized names; for example, HSS field 3 is internally named `hearts` while its localized cost text calls the currency Rings. The HWU frame named `icon_HUD_ring.png` visibly contains the game's diamond currency and is paired with the localized Diamonds label. HWU has no corresponding book or pencil HUD icon nodes, so those labels intentionally remain text-only. The relationship-screen `icon_heart_achromatic.png` is not used as a currency icon; its observed use is in `date_relationship_screen.ccb`.

Atlas frames with the plist `rotated` flag are cropped with their width and height swapped, then rotated 90 degrees counterclockwise to restore the displayed orientation. Dimensions above describe the corrected extracted PNGs.

## Friendly editor section icons

The side-by-side "Edit your game" buttons retain their text labels and show selected-game atlas crops for Classmates, Campus buildings, Campus plots, and Relationships. Plot cards themselves remain icon-free.

| Game | Button | Source frame in `assets\interface-hd.png` | Frame dimensions / atlas metadata | Sandbox icon |
|---|---|---|---|---|
| HSS | Classmates | `button_roster.png` | 60×64; not rotated | `assets\hss\ui\icons\category_classmates.png` |
| HSS | Campus buildings | `button_buildings.png` | 100×104; rotated flag set, restored on extraction | `assets\hss\ui\icons\category_buildings.png` |
| HSS | Campus plots | `education_map_icon.png` | 64×60; not rotated | `assets\hss\ui\icons\category_plots.png` |
| HSS | Relationships | `icon_heart_achromatic.png` | 94×84; rotated flag set, restored on extraction | `assets\hss\ui\icons\category_relationships.png` |
| HWU | Classmates | `button_roster.png` | 60×62; not rotated | `assets\hwu\ui\icons\category_classmates.png` |
| HWU | Campus buildings | `button_buildings.png` | 100×102; not rotated | `assets\hwu\ui\icons\category_buildings.png` |
| HWU | Campus plots | `map_for_sale_sign.png` | 156×296; rotated flag set, restored on extraction | `assets\hwu\ui\icons\category_plots.png` |
| HWU | Relationships | `icon_heart_achromatic.png` | 88×84; rotated flag set, restored on extraction | `assets\hwu\ui\icons\category_relationships.png` |

The roster sprites visibly depict a roster/list (HSS) and character profiles (HWU); the building sprites show a house blueprint (HSS) and a building (HWU). The education map icon and map-for-sale sign were chosen as visually relevant plot/map artwork; the achromatic heart is a relationship icon, not a currency indicator. The atlas frame names and artwork support these category associations. A search of the decompiled `.ccb` and `.lua` files did not find literal references to all section-icon frame names, so this provenance records atlas-frame and visual evidence, not a confirmed scene-node or runtime call-site mapping. The artwork is a direct crop from the read-only original atlases; all extracted files are sandbox copies.

## Specific building card artwork

Building cards use the actual base-building sprite when the selected game's building type maps to a verified frame in its original 2048×2048 building texture atlas. The extracted frame is shown on the card; building types without a matching standalone base sprite retain the generic building category icon. All rotated atlas frames were cropped using swapped source dimensions and rotated 90° counterclockwise. The source decompilation trees were read only.

| Game | Source atlas frame(s) | Sandbox card artwork |
|---|---|---|
| HSS | `building_texture_1_png-hd`: `admissions_1` | `assets\hss\ui\buildings\admissions_1.png` |
| HSS | `building_texture_3_png-hd`: `dorm_artist_1`, `dorm_nerd_1`, `dorm_prep_1`, `dorm_slacker_1` | `assets\hss\ui\buildings\<frame>.png` |
| HSS | `building_texture_4_png-hd`: `matchmaker`, `party`, `polling_building` | `assets\hss\ui\buildings\<frame>.png` |
| HSS | `building_texture_5_png-hd`: `classroom_1`, `dorm_jock_1`, `dorm_musician_1`, `dorm_outdoor_1` | `assets\hss\ui\buildings\<frame>.png` |
| HSS | `building_texture_decoration_png-hd`: `dorm_class_pres_1`, `library` | `assets\hss\ui\buildings\<frame>.png` |
| HWU | `building_texture_1_png-hd`: `admissions_1`, `party`, `workshop` | `assets\hwu\ui\buildings\<frame>.png` |
| HWU | `building_texture_2_png-hd`: `dorm_fashionista_1`, `matchmaker` | `assets\hwu\ui\buildings\<frame>.png` |
| HWU | `building_texture_3_png-hd`: `dorm_director_1`, `dorm_movie_star_1` | `assets\hwu\ui\buildings\<frame>.png` |
| HWU | `building_texture_4_png-hd`: `dorm_monster`, `dorm_pop_star_1`, `dorm_stunt_1` | `assets\hwu\ui\buildings\<frame>.png` |

Frame-to-building mappings were additionally checked against each game's `.ccb` scene references. In particular, the HSS admissions, classroom, Dorm Jock, and Dorm Nerd cards use the corresponding in-game building frame; the HWU Admissions card uses its own game-specific artwork.

## Decoration card artwork

Decoration cards use the selected game's exact sprite frame when a decoration enum maps to a verified frame in that game's building texture atlases. The original source PNG atlases are 2048×2048. Crops use the plist frame rectangle and rotation flag; rotated crops are restored by swapping source width and height, then rotating 90° counterclockwise. Extracted PNGs retain the frame's displayed dimensions. The decompilation directories were read only; all crops below are sandbox copies.

| Game | Source atlas | Extracted frames | Sandbox directory |
|---|---|---|---|
| HSS | `building_texture_1_png-hd` | `bike_rack`, `clock_tower`, `firepit`, `flower_box_fat_short`, `picnic_table`, `rose_trellis` | `assets\hss\ui\decorations\` |
| HSS | `building_texture_2_png-hd` | `asian_lion`, `fountain_cupid`, `lion_statue`, `parade_float`, `pumpkin_patch`, `waterfall` | `assets\hss\ui\decorations\` |
| HSS | `building_texture_4_png-hd` | `carriage`, `lamppost`, `portapotty` | `assets\hss\ui\decorations\` |
| HSS | `building_texture_5_png-hd` | `bench_park01`, `box_of_puppies`, `potted_plant` | `assets\hss\ui\decorations\` |
| HSS | `building_texture_decoration_png-hd` | `asphalt_tile`, `bake_sale_table`, `balloons_gold_silver`, `brick_tile`, `cobblestone_tile`, `cupcake_cart`, `cybersmile`, `dinosaur_skeleton`, `food_truck`, `fountain`, `generic_tree`, `gingerbread_house`, `gold_tile`, `hedge_lg`, `maypole`, `palmtree`, `snack_cart`, `steppingstone_tile`, `topiary_elephant`, `xmas_tree` | `assets\hss\ui\decorations\` |
| HWU | `building_texture_3_png-hd` | `swimming_pool` | `assets\hwu\ui\decorations\` |
| HWU | `building_texture_decoration_png-hd` | `asphalt_tile`, `award_statue`, `bake_sale_table`, `balloons_gold_silver`, `bench_park01`, `bike_rack`, `brick_tile`, `cobblestone_tile`, `dinosaur_skeleton`, `director_chair`, `flower_box_fat_short`, `food_truck`, `fountain`, `generic_tree`, `gold_tile`, `heart_tub`, `hedge_lg`, `lamppost`, `limo_back`, `limo_front`, `limo_middle_1`, `lion_statue`, `marble_tile`, `movie_light`, `palmtree`, `picnic_table`, `portapotty`, `potted_plant`, `red_carpet_tile`, `rose_trellis`, `snack_cart`, `spotlight`, `star_tile`, `steppingstone_tile`, `umbrella_table`, `velvet_rope01`, `wall_brick`, `wall_pillar` | `assets\hwu\ui\decorations\` |

The editor maps the matching HSS and HWU decoration enum symbols to these exact frame filenames (38 HSS and 39 HWU). The same save type can therefore display different artwork under each game's theme. A type without a verified matching frame uses that game's generic decoration icon rather than a guessed sprite. Decoration types remain in the existing buildings collection; this visual change does not add or alter save fields.

## Classmate portraits

The classmate cards use name-matched character portraits cropped from each game's `gamemaker_thumbnails-hd` atlas. The atlas and its `.plist` frame index are 1024×1024; only the named frame rectangles are copied into the sandbox, not the full atlas. The original source trees remain read-only.

| Game | Source | Frames extracted | Sandbox directory | Crop handling |
|---|---|---:|---|---|
| HSS | `HighSchoolStoryRestoredv1.apk\assets\gamemaker_thumbnails-hd.png` + `.plist` | 68 | `assets\hss\ui\portraits\` | Frames retain their indexed names; rotated frames are restored to display orientation |
| HWU | `HollywoodURestoredv1\assets\gamemaker_thumbnails-hd.png` + `.plist` | 93 | `assets\hwu\ui\portraits\` | Frames retain their indexed names; rotated frames are restored to display orientation |

The editor matches `original_name` to a portrait filename (case-normalized), using the display name only when `original_name` is absent, and lazy-loads the image in the matching game theme. If an identity is absent or has no matching portrait, the card displays that game's `button_roster.png` crop (`assets\<game>\ui\icons\category_classmates.png`) as a clearly labeled generic fallback; it does not substitute another character's portrait. This is a visual enhancement only; no save fields or editing behavior change.

## Relationship and classmate progression mapping

The read-only `hsssave.py` and `hwusave.py` protobuf descriptors define `Player.CharacterRelationship.strength` as `int32`, not `fixed32`/float. The editor reads/writes it as a signed varint. Each game's `Config.relationship_levels` gives the status name in `dialog_text` and its `strength` threshold; native `PlayerLogic::getRelationshipLevelForStrength` selects the highest configured threshold not greater than the saved strength. The editor shows a one-based level number and progress as the strength difference from that threshold. Config thresholds are five points apart in both games; the top configured status has no further progress increments. Classmate level mapping uses each game's ordered `CharacterLevelConfig.skill_required` thresholds.

| Game | Source evidence | Verified progression | Editor behavior |
|---|---|---|---|
| HWU | `HollywoodURestoredv1\assets\config.protobin`; native `CharacterLogic::getLevelIndexForSkillPoints` / `getSkillPointsForCharacterAdvance` in the read-only Ghidra export; `assets\help_strings.lua` (`scene_help_level_classmate`) and `assets\tutorial_start.lua` | The tutorial directs the player to select a classmate in the Workshop, wait or rush the timer, then collect to level them. The 100 `CharacterLevelConfig` rows define `skill_required` as 0–99 and `skill_increase` as 1 through level 99 and 0 at level 100; native level display is row index + 1. | Classmate cards show the in-game level and saved skill-point progress to the next configured threshold. Editing a level writes the corresponding `Character.skill_points` threshold. The editor does not edit Workshop actions, timers, or collection state. |
| HSS | `HighSchoolStoryRestoredv1.apk\assets\config.protobin`; embedded `CharacterLevelConfig` descriptor in `libHSS.so`; native `CharacterLogic::getLevelIndexForSkillPoints` / `getSkillLevel` in the read-only Ghidra export; `assets\tutorial_start.lua` | The tutorial says books bought from Classrooms are used to level classmates. The ten `skill_required` thresholds map levels 1–10 to 0, 5, 30, 130, 630, 3,130, 8,130, 18,130, 33,130, and 53,130 skill points; the native lookup chooses the highest threshold not greater than the saved points and displays its row index + 1. Adjacent threshold gaps are 5, 25, 100, 500, 2,500, 5,000, 10,000, 15,000, and 20,000. `skill_increase` is a distinct config field and is not used as the displayed progress denominator. | Classmate cards show the in-game level and progress toward the next threshold. Editing a level writes its `skill_required` value to `Character.skill_points`; Level 10 is the maximum. |

### Dating relationship levels

The read-only game configs expose the exact status names in each relationship level's `dialog_text` and the stored `strength` threshold. Native `PlayerLogic::getRelationshipLevelForStrength` maps a saved strength to the greatest threshold it meets. HSS config has seven statuses (Flirting, Crushing, Online Official, Sweethearts, In Love, Head Over Heels, Over The Moon) with thresholds 0, 5, 10, 15, 20, 25, 30. HWU config has five (Meeting Cute, Having Chemistry, Seen Together, Hooking Up, In The Spotlight) with thresholds 0, 5, 10, 15, 20. The native dating-screen item calls this lookup to display the relationship status. In `DateLogic::resolveDateAction`, the existing-relationship path advances saved strength by one and clamps it at the top configured threshold. Editor progress therefore represents 0–4 strength increments after the selected status threshold; the final status is capped with no further progress control. This maps the existing relationship's `strength` only; date history and date records remain unchanged.

## Backup-based verification

On 2026-10-30, temporary copies of one HSS v5.4.0 and one HWU v3.8.0 save snapshot were tested in the sandbox browser editor. The copies were hash-verified against their source backups before use, and both source files were left unchanged. HSS passed 21 focused checks. HWU passed 19 applicable general checks; its backup contained no saved relationship, so five additional checks exercised relationship creation, all five configured statuses, the strength-20 maximum, and undo using an in-memory relationship. Both sessions ended with the parsed save bytes restored exactly to their loaded state, and the temporary copies were removed. The checks included profile detection, parse/serialize preservation, friendly sections/artwork, representative quick-resource/classmate/building/plot edits, undo, filtering, and an encryption/decryption round-trip.

This evidence is scoped to the tested backups and operations. It is not exhaustive coverage of every raw field, malformed files, mobile browsers, or in-game acceptance of downloaded edits. See [README.md](README.md) for deployment and privacy details.

## Mobile notes

The HTML has responsive layout rules, but phone usability and mobile file import/export have not been device-tested. The editor relies on browser Web Crypto; secure-context requirements and file-picker/download behavior vary by mobile browser. See [README.md](README.md) for the current limitations.

## Reviewed assets not assigned to existing controls

The atlas also contains operation-specific artwork such as building move/rotate/flip/sell buttons, generic colored button plates, character/store art, and additional arrows. They are not wired into the editor because it has no corresponding operations or stable asset-to-save-field mapping; showing them could imply unsupported actions or meanings. The editor uses the verified currency, category, section-banner, panel, control, and matching toolbar-state assets documented above. Broad gameplay atlases and modular clothing/face layers are not copied as UI assets.
