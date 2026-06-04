# Vampire: The Masquerade V5 Kit Player's Guide for SillyTavern

**A complete guide to running the kit in SillyTavern**

Last updated: 2026-06-04
Small changes to Character Creation and Storyteller cards + lorebook

---

<img width="910" height="1172" alt="Screenshot from 2026-06-05 01-18-27" src="https://github.com/user-attachments/assets/f26f33aa-45d2-407f-a128-9e526b36388d" />

---

## Domains

1. **Melbourne** - Camarilla - Prince Marcus Lytton - Toreador
2. **Sydney**    - Independent (non-Camarilla, non-Anarch, non-Sabbat) - Sarrasine - Setite (now Ministry) Methuselah masquesrading as a Tereador
3. **Brisbane**  - Sabbat - Bishop Callista Vox
4. **Adelaide**  - A smaller-domain Camarilla - Prince Octavia Marsh - Ventrue

## Quick Start (TL;DR)

If you want to start playing tonight with minimum setup:

1. **Import these always**: `vtm_v5_storyteller.json` (character) + the entire `VtM base and mechanics lorebook/` folder (7 lorebooks)
2. **Pick one domain**: Import that domain's `_by_night.json` lorebook (e.g., `vtm_chicago_by_night.json`)
3. **Pick one character card from that domain** (e.g., `beckoned_prince.json`)
4. **Chat with the Storyteller character**, attach the lorebooks, and use the character card as your scenario opener

That's it. Everything else in this guide is depth.

---

## What This Kit Is

This kit is a **production-ready chronicle-support package** for running V:tM V5 chronicles in SillyTavern. The kit privileges:

- **Cross-pack institutional integration** — lorebooks reference each other coherently
- **Restraint stance methodology** — cultural-spiritual matters belong to actual communities rather than predetermined kit authority
- **Chronicle-active 2025-2026 operational stakes** — every anchor NPC and institutional axis supports chronicle-scale play
- **Arithmetic and timeline consistency** — verified across all eleven domain lorebooks

The kit is **modular** — you can use as much or as little as you want. The mechanics lorebooks are universal; the domain lorebooks are independent; the character cards within each domain layer onto that domain's lorebook.

---

## Kit Inventory at a Glance

<details>
<summary><strong>📋 Complete kit file listing</strong></summary>

### Core kit (always import)

| File | Purpose |
|---|---|
| `vtm_v5_storyteller.json` | Storyteller character card — your "GM" persona |
| `vtm_v5_character_creation.json` | Character creation guidance lorebook |
| `vtm_v5_character_creator.json` | Character creator character card (alternative to Storyteller for chargen sessions) |

### Mechanics lorebooks (always import)

Located in `VtM base and mechanics lorebook/`:

| File | Purpose |
|---|---|
| `vtm_v5_core_mechanics.json` | Core V5 mechanics (Hunger, dice pools, Resonance, Humanity, etc.) |
| `vtm_v5_disciplines_detailed.json` | All Disciplines and powers |
| `vtm_v5_combat_detailed.json` | Combat mechanics |
| `vtm_v5_rituals_ceremonies.json` | Blood Sorcery and Oblivion rituals |
| `vtm_v5_merits_flaws.json` | Merits, Flaws, Backgrounds |
| `vtm_v5_coterie_creation.json` | Coterie creation guidance |
| `vtm_v5_chronicle_creation.json` | Chronicle creation guidance |
| `vtm_modern_nights.json` | Modern Nights setting context (Second Inquisition, Beckoning, etc.) |

### Domain lorebooks (pick one or more)

Located in `Globe/[Region]/[City]/lorebook/`:

| Lorebook | Domain Type |
|---|---|
| `vtm_sydney_by_night.json` | Sarrasine Independent (methuselah-tempo) |
| `vtm_melbourne_by_night.json` | Lytton Camarilla orthodox |
| `vtm_brisbane_by_night.json` | Bishop Callista Vox Sabbat-survivor |
| `vtm_adelaide_by_night.json` | Octavia Marsh smaller-domain Edwardian Camarilla |
| `vtm_cross_tasman_auckland_wellington.json` | Hartley-Cowan Camarilla + Thornton Anarch Coordination |
| `vtm_berlin_by_night.json` | Three-power-centre Anarch |
| `vtm_london_by_night.json` | Bowesley Westminster Camarilla orthodox |
| `vtm_los_angeles_by_night.json` | Salvador Garcia Council of Barons Anarch |
| `vtm_new_york_by_night.json` | Vandenberg Camarilla reclamation |
| `vtm_tokyo_by_night.json` | Genji Concordat cross-tradition Western-Eastern |
| `vtm_chicago_by_night.json` | Maxwell Camarilla contested mid-tier |

### Supplementary lorebooks (specialized expansion)

| Lorebook | Purpose |
|---|---|
| `vtm_garou_diplomatic.json` (Melbourne) | Garou diplomatic supplement for cross-supernatural play |
| `vtm_glass_walker_npc_pack.json` (Melbourne) | Glass Walker NPCs for Brisbane chronicle-defining moment |
| `vtm_pentex_by_night.json` (Australia) | Pentex corporate antagonist infrastructure |
| `vtm_black_spiral_dancers.json` (Australia) | Black Spiral Dancers antagonist tribe |
| `vtm_russian_far_east_refusenik.json` (Brisbane) | Cardinal Magdalena Volkov network |
| `vtm_pacific_northwest_by_night.json` (Brisbane) | Cardinal Reyna's Continental Corridor |
| `vtm_south_american_highlands_refusenik.json` (Brisbane) | Cardinal Aurelius Tillinghurst network |
| `vtm_cross_pacific_refusenik.json` (Brisbane) | Three-Cardinal Cross-Pacific Refusenik framework |

### Antagonist NPC packs

| Pack | Purpose |
|---|---|
| `vtm_antagonist_npc_pack.json` | Universal antagonist NPC pack (cross-domain) |
| `vtm_australian_antagonist_pack.json` | Australian continental antagonist pack |

### Coterie packs (pre-built coteries by domain)

| Pack | Purpose |
|---|---|
| `vtm_melbourne_coterie_pack.json` | Melbourne pre-built coterie |
| `vtm_sydney_coterie_pack.json` | Sydney pre-built coterie (with 5 individual character cards) |
| `vtm_adelaide_coterie_pack.json` | Adelaide pre-built coterie (with 5 individual character cards) |
| `vtm_brisbane_coterie_pack.json` | Brisbane pre-built coterie (with 5 individual character cards) |

### Chronicle scenario character cards

Located in `Globe/[Region]/[City]/cards/` or scenarios subfolders. Each card is a chronicle scenario you can drop into your campaign.

| Domain | Available scenario cards |
|---|---|
| **Chicago** | Lake Treaty Renewal, Beckoned Prince (Cordelia Crisis), Methuselah Arrives (Ambrogia), Twilight Operation (Donna Lucia/Sol Crisis), Therapist's Couch (Adaeze) |
| **Melbourne** | Lytton's Prince's Charge, Sofia Cress Council, Lumley-Drummond Workings, Red Mag Footscray Question, Sarrasine Sydney Audience |
| **Sydney** | 5 coterie member cards (Eloise, Astrid, Harrison, Nicola, Reggie) |
| **Adelaide** | 5 coterie member cards (Augustin, Saoirse, Alistair, Harriet, Brother Quentin) |
| **Brisbane** | 5 coterie member cards (Tyrell, Brother Owain, Sister Aneka, Templar Annika, Brother Petros) |
| **Cross-Pacific (Brisbane region)** | 5 scenario cards (Brother Robert, Sister Gemma, Elena, Tatiana, Miguel Antonio) |
| **Cross-Wyrm-Infrastructure (Australia)** | 5 scenario cards (Cassandra, Dr. Zara, Madame Yelena, Brother Tomás, Sergeant Eli) |

</details>

---

## SillyTavern Setup Basics

<details>
<summary><strong>🔧 Where to put kit files in SillyTavern</strong></summary>

### Lorebook files

In SillyTavern, lorebooks (also called "World Info" or "World Books") are imported through the **World Info panel**. To use this kit:

1. Open SillyTavern
2. Navigate to **World Info** (book icon in the top bar)
3. Click **Import** and select the lorebook JSON file
4. The lorebook appears in your World Info list

You can also drag-and-drop JSON files directly into the World Info panel.

### Character card files

Character cards are imported through the **Characters panel**:

1. Click the **Characters** icon in the top bar
2. Click **Import Character** (paperclip icon)
3. Select the character JSON file
4. The character appears in your character list

### File locations (for manual placement)

If you prefer to place files directly:
- **Lorebooks (World Info)**: `SillyTavern/data/[your-user]/worlds/`
- **Character cards**: `SillyTavern/data/[your-user]/characters/`

After manual placement, refresh SillyTavern or restart it to load the new files.
</details>

<details>
<summary><strong>🔗 Linking lorebooks to character cards</strong></summary>

SillyTavern supports two ways to associate lorebooks with characters:

### Method 1: Global lorebooks (always active)

For mechanics lorebooks that should always be available:

1. Open **World Info** panel
2. Select the lorebook
3. Check **"Active"** at the top of the panel
4. Set the lorebook to **Global** scope

Recommended for: All mechanics lorebooks (`vtm_v5_core_mechanics`, `vtm_v5_disciplines_detailed`, etc.)

### Method 2: Character-linked lorebooks (activate per character)

For domain-specific lorebooks that should only activate with certain characters:

1. Open the character card
2. In the character settings, find **"Character Lore"** or **"Linked World Info"**
3. Click **"Link"** and select the lorebook
4. The lorebook activates only when chatting with that character

Recommended for: Domain lorebooks (`vtm_chicago_by_night`, etc.) linked to that domain's character cards.

### Method 3: Chat-level lorebooks (activate per chat)

For temporary scenario use:

1. Inside a chat, open the lorebook panel
2. Select lorebooks to activate for this chat only
3. The selection persists for this chat but not others

Recommended for: Crossover scenarios, multi-domain chronicles where you want to switch domain lorebooks mid-chronicle.
</details>

<details>
<summary><strong>⚙️ Recommended SillyTavern settings for V:tM play</strong></summary>

### Context length

The kit lorebooks are dense. Recommended minimum context length:
- **Minimum**: 8K tokens (basic play, single domain)
- **Recommended**: 16K-32K tokens (multi-domain play, deeper institutional engagement)
- **Optimal**: 64K+ tokens (full chronicle continuity with multiple cards + lorebooks)

### Scan depth

Most kit lorebooks have `scan_depth: 4` configured, which means lorebook entries trigger based on keywords in the last 4 messages. You can override this in the World Info settings if your context budget allows higher scan depth.

### Token budget

The kit lorebooks have `token_budget: 2400` configured. This means up to 2400 tokens of lorebook content can be injected per message. Adjust based on your model's context length:
- For 8K context: Reduce to ~1500
- For 16K+ context: 2400 is comfortable
- For 64K+ context: You can raise to 4000+ for very rich institutional context

### Recursive scanning

Most kit lorebooks have `recursive_scanning: false`. This means lorebook entries don't trigger from other lorebook entries' content. This keeps token budgets predictable. Leave it off unless you specifically want deeper auto-triggering.

### Model recommendations

The kit was developed assuming high-quality language models. Recommended:
- **Best**: Claude Sonnet 4.5, Claude Opus 4 / 4.1, GPT-5, Gemini 2.5 Pro
- **Good**: Claude Sonnet, GPT-4o, Gemini 2.5 Flash
- **Workable**: Llama 3.1 70B+, Mistral Large, smaller Claude/GPT models
- **Limited**: 7B-13B local models may struggle with kit's institutional density
</details>

---

## How to Run a Chronicle

There are three primary ways to use this kit. Pick the one that matches your play style.

### Mode 1: Single-Domain Chronicle (Recommended for Beginners)

Run a chronicle set entirely in one city.

<details>
<summary><strong>Mode 1 setup walkthrough</strong></summary>

**Step 1: Pick a domain.**

Each domain has a distinct faction register. Match the register to your preferred play style:

| If you want... | Pick domain | Faction register |
|---|---|---|
| Classic Camarilla intrigue | London or Melbourne | Camarilla orthodox |
| Contested cross-faction politics | Chicago | Camarilla mid-tier vs. Anarchs vs. Hecata |
| Anarch revolution chronicle | LA or Berlin | Council of Barons / three-power-centre |
| Post-Sabbat-dominion reclamation | NYC | Camarilla reclamation |
| Sabbat-survivor / cross-supernatural | Brisbane | Sabbat-survivor + Cress Truce |
| Methuselah-tempo Independent | Sydney | Sarrasine domain |
| Cross-tradition Western-Eastern | Tokyo | Genji Concordat |
| Smaller-domain Edwardian register | Adelaide or Auckland | Smaller-domain Camarilla |

**Step 2: Import the essentials.**

- All mechanics lorebooks (8 files in `VtM base and mechanics lorebook/`)
- The Storyteller character (`vtm_v5_storyteller.json`)
- Your chosen domain's `_by_night.json` lorebook

**Step 3: Create your character.**

Use the Character Creator character (`vtm_v5_character_creator.json`) or build manually with the character creation lorebook.

If your domain has a coterie pack (Sydney, Adelaide, Brisbane, Melbourne), you can:
- Use pre-built coterie members as PCs, or
- Use the coterie pack as a template for your custom PCs

**Step 4: Start a chronicle session.**

- Chat with the Storyteller character, OR
- Chat directly with a domain character card (e.g., Cordelia Whitmore-Ash) to drop into that scenario

**Step 5: Layer scenario cards as chronicle progresses.**

Most domain lorebooks have associated scenario character cards. As your chronicle advances, introduce scenario cards to bring chronicle-defining moments into play.
</details>

### Mode 2: Cross-Pack Multi-Domain Chronicle (Intermediate)

Run a chronicle that spans multiple domains through documented institutional channels.

<details>
<summary><strong>Mode 2 setup walkthrough</strong></summary>

**Step 1: Pick a primary domain.**

Your chronicle's "home base." All other domains will be visited or referenced through cross-pack channels.

**Step 2: Identify your cross-pack axes.**

Your chronicle will likely use 2-4 of the kit's documented cross-pack institutional axes:

| Cross-pack axis | Domains | Subject matter |
|---|---|---|
| **Anglosphere Camarilla princely peer circle** | Melbourne + London + Auckland + Adelaide + NYC + Chicago | Princely-peer correspondence, trajectory disclosure |
| **Ventrue financial-services axis** | Tokyo + London + NYC + Chicago | Financial-services clan coordination |
| **Hecata family network** | NYC + London + Chicago + Sicily (Ambrogia) + Calabria | Family-formal correspondence |
| **Cross-domain Nosferatu network** | London + NYC + LA + Tokyo + Brisbane + Chicago | Nosferatu intelligence-sharing |
| **Three-city Banu Haqim diaspora axis** | Berlin + LA + Tokyo | Damascene-Istanbul diaspora coordination |
| **Trans-Atlantic Carna-defence axis** | Berlin + London + NYC + Chicago | Tremere Carna-aligned faction defence |
| **Cross-coastal Anarch Brujah network** | LA + Chicago + Berlin + Wellington | Brujah Anarch coordination |
| **Toreador cultural-production axis** | LA + NYC + Tokyo + Chicago | Cultural-production cross-tradition |
| **Cross-Pacific Refusenik framework** | Brisbane + Pacific Northwest + Russian Far East + South American Highlands | Three-Cardinal Sabbat-refusenik coordination |
| **Cress Truce framework** | Brisbane + Australian continental + Cross-Tasman | Cross-supernatural diplomatic |

**Step 3: Import the lorebooks for your axes.**

For each axis you've selected, import the relevant domain lorebooks. For deep Hecata-focused chronicles, you'd import NYC + London + Chicago. For Banu Haqim diaspora chronicles, Berlin + LA + Tokyo.

**Step 4: Manage context budget carefully.**

Multi-domain chronicles run hot on context. Strategies:
- Increase context length if your model supports it
- Set non-primary domain lorebooks to lower priority
- Disable lorebooks for domains not currently active in the scene
- Use chat-level lorebook activation (Method 3 above) to swap domain lorebooks as scenes change

**Step 5: Run cross-pack scenarios.**

Use the kit's documented chronicle-defining moments as cross-pack scenarios:
- **October 2026 Brisbane Glass Walker** — produces institutional attention across multiple domains
- **Cardinal Tillinghurst May 2026 succumbence** — Cross-Pacific Refusenik chronicle climax
- **August/September/October 2025 Disciplines** — Second Inquisition synchronous response across Berlin, NYC, London
</details>

### Mode 3: Cross-Supernatural Chronicle (Advanced)

Engage Werewolf: The Apocalypse content alongside V:tM through the Garou diplomatic supplement.

<details>
<summary><strong>Mode 3 setup walkthrough</strong></summary>

**Step 1: Import cross-supernatural lorebooks.**

- All standard V:tM mechanics
- Your chosen V:tM domain
- `vtm_garou_diplomatic.json` (Melbourne Garou Diplomatic Supplement)
- `vtm_glass_walker_npc_pack.json` (if engaging the Brisbane Glass Walker chronicle-defining moment)
- `vtm_pentex_by_night.json` (corporate antagonist infrastructure)
- `vtm_black_spiral_dancers.json` (antagonist tribe)

**Step 2: Frame the chronicle around the Cress Truce framework.**

The Cress Truce is the kit's documented cross-supernatural diplomatic infrastructure spanning Australian continental + Cross-Tasman domains. Frame your chronicle around:
- Diplomatic negotiation between Kindred domains and Garou tribes
- Cross-supernatural responses to Pentex corporate threats
- Black Spiral Dancers as cross-supernatural antagonist threat
- October 2026 Brisbane Glass Walker chronicle-defining moment

**Step 3: Use Cross-Wyrm-Infrastructure scenario cards.**

The `Cross-Wyrm-Infrastructure Chronicle Scenarios — Five Character Cards/` folder contains scenario cards specifically designed for this play mode:
- Cassandra Webb-Lin
- Dr. Zara Okonkwo-Hartwell
- Madame Yelena Hasanov-Chen
- Brother Tomás Cortez-Walsh
- Sergeant Eli Mahonen-Keough

**Restraint stance note**: Cross-supernatural play engages Garou tribal heritage and other culturally-specific supernatural traditions. The kit's restraint stance framework applies — Garou tribal cosmology and Indigenous heritage matters belong to actual communities and institutional voices rather than predetermined kit authority.
</details>

---

## Domain Selection Guide

Detailed comparison of each domain's chronicle character.

<details>
<summary><strong>🇦🇺 Australian Continental Domains</strong></summary>

### Sydney (Sarrasine Independent)

- **Senior figure**: Sarrasine (1,470-year tenure, methuselah-tempo)
- **Faction**: Independent methuselah domain
- **Tone**: Slow-paced, deeply-rooted, methuselah-scale institutional gravity
- **Best for**: Chronicles where {{user}}'s actions ripple across centuries; cross-Pacific diplomatic work
- **Coterie pack available**: Yes (5 cards)
- **Key cross-pack channel**: Decourcelle-Sarrasine (Tokyo), Aldington-Sarrasine (Tokyo)

### Melbourne (Lytton Camarilla orthodox)

- **Senior figure**: Prince Lytton (235-year tenure, intermediate Beckoning)
- **Faction**: Camarilla orthodox
- **Tone**: Classic Camarilla domain with Anglosphere senior figure framework
- **Best for**: Classic V:tM chronicle play with rich institutional politics
- **Coterie pack available**: Yes
- **Special supplements**: Garou Diplomatic, Glass Walker NPC Pack
- **Scenario cards**: 5 (Lytton's Prince's Charge, Sofia Cress Council, Lumley-Drummond Workings, Red Mag Footscray Question, Sarrasine Sydney Audience)

### Adelaide (Octavia Marsh smaller-domain Edwardian Camarilla)

- **Senior figure**: Octavia Marsh (163-year tenure, intermediate Beckoning)
- **Faction**: Smaller-domain Edwardian Camarilla
- **Tone**: Intimate, atmospheric, Edwardian-period institutional register
- **Best for**: Chronicles with deep mortal-community engagement, smaller cast
- **Coterie pack available**: Yes (5 cards)
- **Restraint stance: Indigenous Australian heritage (Kaurna, Peramangk) explicitly applied**

### Brisbane (Bishop Callista Vox Sabbat-survivor)

- **Senior figure**: Bishop Callista Vox (213 years, 7th gen Tzimisce, methuselah-track Vicissitude 7)
- **Faction**: Sabbat-survivor (post-1976)
- **Tone**: Heterodox, post-Wallachian aesthetic preservation, cross-supernatural anchor
- **Best for**: Sabbat-survivor chronicles, cross-Pacific Refusenik framework engagement, Glass Walker cross-supernatural play
- **Coterie pack available**: Yes (5 cards)
- **Cross-Pacific Refusenik framework anchor**
- **October 2026 Brisbane Glass Walker chronicle-defining moment anchor**
</details>

<details>
<summary><strong>🇳🇿 Cross-Tasman Domain</strong></summary>

### Auckland / Wellington (Hartley-Cowan Camarilla + Thornton Anarch Coordination)

- **Senior figures**: Hartley-Cowan (Auckland Prince, 178 years), Maggie Thornton (Wellington Coordination Council, 127 years)
- **Faction**: Dual — Camarilla smaller-domain (Auckland) + Anarch Coordination (Wellington)
- **Tone**: Cross-Tasman institutional collaboration with Māori-lineage and Pacific Islander community context
- **Best for**: Cross-faction chronicles, smaller-domain Anglosphere institutional play
- **Restraint stance: Māori-lineage Kindred (Hēmi Whatutua), Pacific Islander diaspora explicitly applied**
</details>

<details>
<summary><strong>🇩🇪 Berlin (Three-Power-Centre Anarch)</strong></summary>

- **Senior figures**: Anneliese Brandt (Brujah Council), Magdalena Fuchs (Tempelhof Carna Library), Yusuf Demir (Kreuzberg Banu Haqim diaspora, acute Beckoning)
- **Faction**: Three-power-centre Anarch (three independent power centres coordinate)
- **Tone**: Politically dynamic, multi-clan Anarch coordination, trans-Atlantic Carna-defence stakes
- **Best for**: Anarch chronicle play with complex internal politics, trans-Atlantic institutional engagement
- **Key cross-pack axes**: Three-city Banu Haqim diaspora (with LA + Tokyo), trans-Atlantic Carna-defence (with London + NYC + Chicago)
- **Restraint stance: Turkish-German Islamic religious practice explicitly applied**
</details>

<details>
<summary><strong>🇬🇧 London (Bowesley Westminster Camarilla)</strong></summary>

- **Senior figure**: Prince Bowesley (469-year tenure, preliminary intermediate Beckoning)
- **Faction**: Westminster Camarilla orthodox
- **Tone**: Deep-rooted institutional gravity, Anglosphere senior framework, post-Second-Inquisition pressure
- **Best for**: Classic Camarilla chronicle with deep historical and cross-pack institutional engagement
- **Key cross-pack axes**: Anglosphere princely circle, Ventrue financial-services, Hecata family network, Nosferatu cross-domain, Carna-defence
- **October Restrictions 2025 anchor**
- **Restraint stance: Caribbean-British community explicitly applied**
</details>

<details>
<summary><strong>🇺🇸 Los Angeles (Salvador Garcia Council of Barons)</strong></summary>

- **Senior figure**: Salvador Garcia (279-year tenure, Anarch Movement-architect)
- **Faction**: Anarch Council of Barons
- **Tone**: Multi-Baron Anarch coordination, Hollywood Touchstone Protocol cultural-production register
- **Best for**: Anarch chronicle with cultural-production institutional engagement
- **Key cross-pack axes**: Three-city Banu Haqim diaspora, Toreador cultural-production, Nosferatu cross-domain, cross-coastal Anarch Brujah
- **Restraint stance: Mexican-American Catholic religious practice, Korean-American (Koreatown), Indigenous heritage where applicable explicitly applied**
</details>

<details>
<summary><strong>🇺🇸 NYC (Vandenberg Camarilla Reclamation)</strong></summary>

- **Senior figure**: Prince Augusta Vandenberg (288 years, below-threshold Beckoning, Inner Circle direct mandate)
- **Faction**: Camarilla reclamation (post-Sabbat-dominion since 2020)
- **Tone**: Reclamation-period political fragility, persistent Sabbat-loyalist remnants under Vorbescu
- **Best for**: Post-Sabbat-dominion reclamation chronicle, Hecata family work, cross-faction Tzimisce institutional axis
- **Key cross-pack axes**: Anglosphere princely circle, Ventrue financial-services, Hecata family network (senior North American), Nosferatu cross-domain, Carna-defence, Tzimisce institutional axis
- **September Discipline 2025 anchor**
- **Restraint stance: Caribbean-American, Greek-American, Bangladeshi-American, multi-Latinx, Romanian-American, Italian-American Catholic explicitly applied**
</details>

<details>
<summary><strong>🇯🇵 Tokyo (Genji Concordat Cross-Tradition)</strong></summary>

- **Senior figures**: Magistrate Tachibana Kaname (Eastern Kindred, ~380 years institutional age), Madame Hélène Decourcelle (Western administrator, 209 years)
- **Faction**: Genji Concordat (1872) cross-tradition Western-Eastern accommodation
- **Tone**: Cross-tradition diplomatic, Concordat-constrained Western Kindred presence, Kuei-jin court institutional weight
- **Best for**: Cross-tradition chronicles, Pacific Rim institutional engagement, immigration / refugee plotlines (Hong Kong arrivals)
- **Key cross-pack axes**: Decourcelle-Sarrasine (cross-tradition Western), Ventrue financial-services, three-city Banu Haqim diaspora, Nosferatu cross-domain, Toreador cultural-production
- **Restraint stance: Eastern Kindred / Wan Kuei cosmology (kit-canonical exemplar), Japanese cultural-spiritual matters, Shinjuku Middle Eastern-Japanese / Islamic religious practice explicitly applied**
</details>

<details>
<summary><strong>🇺🇸 Chicago (Maxwell Camarilla Contested Mid-Tier)</strong></summary>

- **Senior figures**: Prince Maxwell Holloway-VanCort (8th gen, 21-year Praxis since 2004), Cordelia Whitmore-Ash (Toreador Harpy, 258 years), Sol Vega-Chen (Pilsen Anarch Baron), Donna Lucia Giovanni-Costa (Hecata matriarch), Ambrogia Giovanni (senior Hecata family figure, 458 years)
- **Faction**: Contested mid-tier — Camarilla heartland (North Side) + Anarch South Districts + Hecata Bridgeport + Tremere Hyde Park
- **Tone**: Uneasy equilibrium under Lake Treaty (1957), Twilight Project Carruth surveillance pressure, chronicle-defining November sequence
- **Best for**: Cross-faction chronicles, faction-choice play (Camarilla / Anarch / Hecata), compressed-time crisis chronicles
- **Key cross-pack axes**: Anglosphere princely circle, Ventrue financial-services, Hecata family network, trans-Atlantic Carna-defence, cross-coastal Anarch Brujah, Nosferatu cross-domain
- **Scenario cards**: 5 (Lake Treaty Renewal, Beckoned Prince, Methuselah Arrives, Twilight Operation, Therapist's Couch)
- **Restraint stance: Mexican-American Catholic religious practice, African-American Chicago South Side, Black-American/Chicago South Shore, Vietnamese-American (Sgt. Lin), Italian-American Catholic, Nigerian-American/Igbo (Adaeze) explicitly applied**
</details>

---

## Chronicle Structure Recommendations

### Single-Domain Chronicle Arc (Recommended Beginner Path)

A complete chronicle in one domain typically runs 10-15 sessions. Recommended structure:

<details>
<summary><strong>Sample 12-session Chicago chronicle arc</strong></summary>

**Sessions 1-2: Faction choice and grounding**
- Use Cordelia scenario card (Camarilla path), Sol scenario card (Anarch path), or Donna Lucia scenario card (Hecata path)
- Establish PC's domain position, initial Touchstones, basic operational competence

**Sessions 3-4: Mortal anchor**
- Use Helen Achebe scenario card (if Camarilla, building Touchstone)
- Use Imogen Wren scenario card (Glass Door integration)
- Or develop custom mortal anchors through clinical practice / community embedding

**Sessions 5-6: Cross-sect politics (March)**
- Lake Treaty Renewal scenario card
- Establish {{user}}'s position in cross-sect institutional architecture
- This scenario runs in March, 8 months before November chronicle-defining events

**Sessions 7-8: First crisis (November Tuesday)**
- Twilight Operation scenario card (compressed-time crisis 2:47 AM Tuesday)
- {{user}} either extracts wraith-archive (Hecata path) or runs tunnel evacuation (cross-sect path)

**Sessions 9-10: Hidden plot or succession crisis**
- Therapist's Couch scenario card (if Helen plot in continuity) — clinical disclosure + Helen-plot convergence
- OR Beckoned Prince scenario card (Cordelia Crisis, Wednesday 3:14 AM following Maxwell's Tuesday 11:18 PM succumbence)

**Sessions 11-12: Climactic assessment**
- Methuselah Arrives scenario card (Ambrogia Giovanni formal Hecata family assessment, Thursday 9:14 PM)
- Defines {{user}}'s standing in the global Hecata family for a century
- Chronicle-climactic stakes

The full chronicle continuity arc is documented in the kit's scenario chart. Chronicle facilitators may run in different order if desired.
</details>

### Multi-Domain Chronicle Arc (Intermediate Path)

<details>
<summary><strong>Sample multi-domain chronicle: Trans-Atlantic Hecata family work</strong></summary>

A chronicle spanning Chicago + NYC + London + Sicily (Ambrogia) through Hecata family network:

**Phase 1 — Chicago grounding (Sessions 1-4)**
- Donna Lucia scenario card establishes {{user}} as Hecata family member
- Maria Costa-Velazquez killing investigation begins
- Costa Funeral Services political-institutional work

**Phase 2 — NYC cross-pack travel (Sessions 5-7)**
- {{user}} travels to NYC Manhattan Branch (Capo Giovanni-Marlowe)
- Cross-family-formal correspondence delivery
- Engagement with Vandenberg's reclamation administration on Hecata-Camarilla cross-faction matters

**Phase 3 — London cross-pack travel (Sessions 8-10)**
- {{user}} travels to London Whitechapel Branch (Capo Ashcroft)
- Bowesley Westminster Camarilla institutional engagement
- October Restrictions 2025 Second Inquisition pressure response

**Phase 4 — Twilight Operation return (Sessions 11-13)**
- {{user}} returns to Chicago for the November Tuesday Twilight Project strike
- Wraith-archive extraction
- Costa Funeral Services destruction

**Phase 5 — Ambrogia assessment + climax (Sessions 14-15)**
- Ambrogia arrives from Sicily, formal family assessment
- Chronicle-defining outcome — {{user}}'s standing in global Hecata family for the next century
</details>

### Cross-Supernatural Chronicle Arc (Advanced Path)

<details>
<summary><strong>Sample cross-supernatural chronicle: Brisbane Glass Walker October 2026</strong></summary>

A chronicle building toward the kit's October 2026 chronicle-defining moment:

**Phase 1 — Brisbane grounding (Sessions 1-3)**
- Bishop Callista Vox introduces {{user}} to Sabbat-survivor domain
- Cress Truce framework introduction
- Cross-supernatural diplomatic context establishment

**Phase 2 — Glass Walker engagement (Sessions 4-6)**
- Glass Walker NPC pack introduces {{user}} to Garou tribal context
- Pentex corporate antagonist infrastructure engagement
- Initial cross-supernatural negotiation work

**Phase 3 — Cross-Pacific Refusenik framework (Sessions 7-9)**
- Cardinal Reyna (Pacific Northwest), Cardinal Tillinghurst (South American Highlands), Cardinal Magdalena (Russian Far East) introduction
- Cross-Pacific Refusenik chronicle infrastructure engagement
- May 2026 Tillinghurst succumbence engagement

**Phase 4 — Pre-climax preparation (Sessions 10-11)**
- Cross-Wyrm-Infrastructure character cards engagement
- Black Spiral Dancers antagonist threat escalation
- Cross-supernatural coalition formation

**Phase 5 — October 2026 climax (Sessions 12-15)**
- Brisbane Glass Walker chronicle-defining operation
- Cross-Pacific institutional disturbance spans multiple kit domains
- {{user}}'s actions ripple across Sydney, Auckland, Wellington, Tokyo, NYC, London, Berlin, LA, Chicago through documented cross-pack channels
</details>

---

## Using Character Cards Effectively

<details>
<summary><strong>🎭 NPC packs vs. coterie packs vs. scenario cards</strong></summary>

The kit has three types of character card content:

### NPC packs (antagonist + universal)

- **Files**: `vtm_antagonist_npc_pack.json`, `vtm_australian_antagonist_pack.json`, `vtm_glass_walker_npc_pack.json`
- **Use**: These are bulk NPC catalogues for the Storyteller to deploy as needed. Import alongside your mechanics lorebooks and treat as on-demand NPC references.
- **Chronicle use**: Storyteller pulls NPCs from these packs as situations arise. Not for direct chat use.

### Coterie packs (pre-built coterie infrastructure)

- **Files**: `vtm_sydney_coterie_pack.json`, `vtm_adelaide_coterie_pack.json`, `vtm_brisbane_coterie_pack.json`, `vtm_melbourne_coterie_pack.json`
- **Use**: Pre-built coterie templates with associated character cards for individual coterie members.
- **Chronicle use**: 
  - **Solo play**: {{user}} plays one coterie member; others operate as Storyteller-controlled supporting characters
  - **Multi-player play**: Each player adopts one coterie member; Storyteller coordinates
  - **Template use**: Use the coterie pack as inspiration for custom coterie creation

### Scenario character cards (chronicle-active scenarios)

- **Files**: Individual `.json` files in `cards/` folders
- **Use**: Chronicle-active scenarios with chronicle-defining stakes. Each card is a complete scenario opener.
- **Chronicle use**: Drop into chronicle when ready to run that scenario. Each card has detailed scenario context, character build, system prompt, mes_example, and alternate greetings.

The Chicago scenario cards are the most extensively developed scenario card set in the kit; the Australian (Melbourne, Sydney, Adelaide, Brisbane) coterie packs provide pre-built coterie templates.
</details>

<details>
<summary><strong>🎬 How to use scenario cards in SillyTavern</strong></summary>

Each scenario card is designed as a single dramatic scene with chronicle-defining stakes. To use:

1. **Import the card** through SillyTavern Characters panel
2. **Link the appropriate lorebook** (e.g., for Chicago scenario cards, link `vtm_chicago_by_night.json`)
3. **Verify mechanics lorebooks are active** as global lorebooks
4. **Start chat with the card** — the first_mes will set the scene
5. **Engage the scenario** — respond to the opening prompt
6. **Use alternate greetings** for variations or sequel scenes

Each card includes:
- `description`: Full character + scenario context
- `personality`: Character's psychological register
- `scenario`: Setting and timing
- `first_mes`: Opening message that establishes the scene
- `mes_example`: Sample exchanges showing tone and structure
- `system_prompt`: Storyteller instructions for running the character
- `alternate_greetings`: 1-2 alternate scenarios (often "six weeks later" or "twelve months later" follow-ups)

### Scenario card chronicle continuity

Cards within a domain are designed to interlock. For example, the Chicago cards operate in this chronicle continuity:

| Order | Card | Date | Dependencies |
|---|---|---|---|
| 1 | Lake Treaty Renewal | March (third Saturday) | Faction loyalty established |
| 2 | Twilight Operation | November Tuesday 2:47 AM | Hecata or contingency network |
| 3 | Beckoned Prince | November Wednesday 3:14 AM | Cordelia relationship |
| 4 | Therapist's Couch | November Tuesday evening | Helen scenario in continuity |
| 5 | Methuselah Arrives | November Thursday 9:14 PM | Hecata family role accepted |
</details>

<details>
<summary><strong>🎙️ Storyteller character vs. direct character chat</strong></summary>

### Storyteller character (`vtm_v5_storyteller.json`)

- **Purpose**: Acts as your GM, narrating scenes, voicing multiple NPCs, adjudicating mechanics
- **Best for**: Open-ended chronicle play, multi-character scenes, mechanics-heavy sessions
- **How to use**: Chat with the Storyteller character with all lorebooks active; describe your action and let the Storyteller narrate the response

### Direct character chat (scenario cards, coterie members)

- **Purpose**: One-on-one focused interaction with a specific character
- **Best for**: Intimate scenes, single-character scenarios, scenario card dramatic moments
- **How to use**: Chat directly with the character card; the character responds in-character

### Hybrid approach (recommended)

Many players use both:
- **Storyteller for cross-scene narration and multi-NPC scenes**
- **Scenario character cards for dramatic single-character scenes**

You can switch between characters mid-chronicle. The lorebooks remain active across all characters as long as they're set to global or linked to the active character.
</details>

---

## Common Issues and Solutions

<details>
<summary><strong>⚠️ "The model is confused about which faction the city is in"</strong></summary>

**Cause**: Multiple domain lorebooks active simultaneously without scene-context disambiguation.

**Solution**:
- Use chat-level lorebook activation (deactivate non-relevant domain lorebooks)
- OR: In your first message, explicitly state the domain ("We're in Chicago Camarilla...")
- OR: Use the Storyteller character with system prompt clarifying domain
</details>

<details>
<summary><strong>⚠️ "The model doesn't know about the Vienna 2019 collapse" (or other kit-specific facts)</strong></summary>

**Cause**: Lorebook entry not triggering because keywords aren't in recent context.

**Solution**:
- Lorebook entries trigger on keywords in `scan_depth` recent messages (default 4)
- Mention the relevant keyword to trigger the entry ("Tell me about the Vienna chantry collapse")
- OR: Set important entries to `constant: true` in the lorebook (always-active)
- OR: Increase `scan_depth` in lorebook settings
</details>

<details>
<summary><strong>⚠️ "I'm running out of context length"</strong></summary>

**Cause**: Too many lorebooks active with high token budgets.

**Solutions** (in order of preference):
1. Use a model with larger context (Claude Sonnet 4.5, GPT-5, Gemini 2.5 Pro all support 200K+ tokens)
2. Lower `token_budget` in active lorebooks
3. Deactivate lorebooks not needed for current scene
4. Use chat-level lorebook activation to swap lorebooks as scenes change
5. Reduce `scan_depth` to limit how many recent messages trigger entries
</details>

<details>
<summary><strong>⚠️ "The model is appropriating cultural-spiritual content"</strong></summary>

**Cause**: Restraint stance methodology not being respected by the model.

**Solutions**:
- Ensure restraint stance language is present in the active lorebook entries (it should be in the kit's rewritten entries)
- Add to your system prompt: "Apply the kit's restraint stance methodology — cultural-spiritual matters belong to actual communities and institutional voices rather than predetermined kit authority"
- Reference the Tokyo Eastern Kindred / Wan Kuei handling as the kit-canonical exemplar
- If the model continues to overstep, redirect explicitly: "Let's keep cultural-spiritual matters as institutional context rather than direct kit-authored religious content"
</details>

<details>
<summary><strong>⚠️ "The model is inventing NPCs not in the lorebook"</strong></summary>

**Cause**: Model creativity producing characters outside kit canon.

**Solutions**:
- This is sometimes desirable! Novel NPCs add chronicle flavor
- If problematic: Add to system prompt "Reference only NPCs documented in the active lorebooks; do not invent new senior figures"
- For senior figures (Princes, Barons, Bishops, Capos, Magistrates), explicitly redirect
- Junior NPCs (mortal contacts, minor Kindred) — invention is fine and expected
</details>

<details>
<summary><strong>⚠️ "Chronicle continuity is getting confused" (Maxwell alive in one scene, succumbed in another)</strong></summary>

**Cause**: Multi-scenario continuity tracking issue.

**Solutions**:
- Reference the chronicle timeline table (see Kit Canon document) for verified ordering
- For Chicago specifically: Lake Treaty (March) precedes the November sequence (Twilight Operation Tuesday 2:47 AM → Maxwell succumbence Tuesday 11:18 PM → Cordelia consultation Wednesday 3:14 AM → Ambrogia assessment Thursday 9:14 PM)
- Explicitly note "Chronicle is currently set in [date]" at the start of each session
- The Storyteller character can be primed with chronicle-state notes between sessions
</details>

---

## Tips for Specific Play Styles

<details>
<summary><strong>For Solo Players</strong></summary>

- The Storyteller character is your primary GM
- {{user}} represents your single PC
- Use coterie packs as supporting NPCs the Storyteller controls
- Scenario cards work well as dramatic punctuation between Storyteller-led sessions
- Recommend single-domain chronicle for first time, then expand to multi-domain
</details>

<details>
<summary><strong>For Multi-Player Groups</strong></summary>

- SillyTavern supports group chats — multiple players can share a session
- Each player gets a PC character; one player (or the AI) plays the Storyteller
- Coterie packs work especially well — each player adopts one coterie member
- Cross-pack chronicles work well with larger groups since multiple players can engage different domains

### Setting up a group chat

1. Create a group chat in SillyTavern (Groups feature)
2. Add the Storyteller character
3. Add PC character cards (one per player, or shared if players want to swap)
4. Activate domain + mechanics lorebooks at group-chat level
5. Players take turns posting in-character; Storyteller responds
</details>

<details>
<summary><strong>For Long-Form Chronicles (50+ sessions)</strong></summary>

- Use chronicle log files to track state between sessions
- The kit's chronicle-active window is October 2025 - October 2026; for chronicles extending beyond, document timeline progression manually
- Multi-domain chronicles benefit from chronicle-state tracking documents alongside SillyTavern chat history
- Consider extracting your chronicle's specific institutional facts (which Praxis Cordelia chose, which faction {{user}} joined, etc.) into a custom personal lorebook for your chronicle

### Personal chronicle lorebook template

Create a new lorebook with entries documenting:
- {{user}}'s clan, generation, sect, current status
- Key Touchstones with current status
- Faction loyalty and contingency-card relationships
- Documented institutional positions held
- Chronicle timeline (what's happened, what's upcoming)
- NPC relationship states (warm, neutral, hostile, etc.)

Set this lorebook to always-active. The Storyteller will reference it across all sessions.
</details>

<details>
<summary><strong>For Short-Form One-Shots</strong></summary>

- Pick a single scenario card and run it as a 1-3 session one-shot
- The Chicago scenario cards work especially well as one-shots — each is designed as a complete dramatic scene
- The Beckoned Prince (Cordelia Crisis) and Methuselah Arrives (Ambrogia) cards are particularly suited to focused one-shot play
- For one-shots, you don't need the full mechanics lorebook suite — basic mechanics + the scenario's domain lorebook is sufficient
</details>

---

## Quick Reference: Restraint Stance

The kit's restraint stance methodology applies across all lorebooks and scenario cards. The Tokyo Eastern Kindred / Wan Kuei handling is the kit-canonical exemplar.

<details>
<summary><strong>Restraint stance — what it means and how to use it</strong></summary>

### The five-point restraint stance framework

1. **Institutional reference without cosmological authority** — Reference V5 published canon (Wan Kuei, Indigenous heritage, Catholic religious practice, Islamic religious practice, etc.) without claiming definitive cosmological or theological authority
2. **Setting-flexible cosmology** — Treat specific supernatural-theological detail as setting-flexible; kit supplies institutional architecture rather than cosmological detail
3. **Community institutional self-determination preserved** — Treat community awareness, Masquerade-protective community attention, and community institutional self-determination as operational structure without instrumentalizing communities as Kindred operational terrain
4. **Explicit acknowledgment over implicit framing** — Where chronicle handling engages cultural-spiritual matters, explicit restraint stance acknowledgment is preferred
5. **Reference exemplars** — The Tokyo Eastern Kindred handling provides the kit-canonical methodology model

### Applications across the kit

- Indigenous Australian heritage (Adelaide, Cross-Tasman)
- Māori-lineage Kindred (Cross-Tasman)
- Pacific Islander diaspora (Cross-Tasman)
- Caribbean-British / Caribbean-American (London, NYC)
- Mexican-American Catholic religious practice (LA, Chicago)
- Korean-American (LA Koreatown)
- Turkish-German Islamic religious practice (Berlin Kreuzberg)
- Vietnamese-American (Chicago Sgt. Lin)
- African-American Chicago South Side (Chicago)
- Italian-American Catholic religious practice (multiple)
- Nigerian-American / Igbo (Chicago Adaeze)
- Eastern Kindred / Wan Kuei cosmology (Tokyo — exemplar)
- Romanian-American (NYC Vorbescu Touchstone)
- And more — see `kit_canon.md` Restraint Stance Application Table

### In play

If a scene engages cultural-spiritual or community matters:
- Treat the cultural-community context as institutional structure
- Don't claim definitive theological / cosmological authority
- Engage community contexts (parish priests, religious-order correspondents, immigrant-community institutional embedding) as documented kit infrastructure
- Preserve community institutional self-determination — communities are not Kindred operational terrain
</details>

---

## Where to Find More

| Document | Location | Purpose |
|---|---|---|
| `kit_canon.md` | Project root | Full kit institutional reference, anchor NPC documentation, cross-pack axes, chronicle timeline |
| `vtm_v5_chronicle_creation.json` | Mechanics lorebook | Chronicle creation guidance |
| `vtm_v5_coterie_creation.json` | Mechanics lorebook | Coterie creation guidance |
| `vtm_modern_nights.json` | Mechanics lorebook | Modern Nights setting context |

For questions about specific NPCs, institutional axes, or chronicle-defining moments, the `kit_canon.md` document is the definitive reference.

---

## Final Notes

This kit was developed with extensive consistency verification across eleven domain lorebooks and dozens of character cards. The kit is **production-ready** at chronicle scale — every senior NPC's age, generation, and tenure is arithmetically verified; cross-pack institutional channels operate at documented tempos; chronicle-defining moments are timeline-reconciled; restraint stance applications are explicit where engaged.

The kit is also **modular**. You don't need to use everything. Pick the domains, scenario cards, and supplementary lorebooks that match your chronicle. The kit is designed to scale from one-shot scenarios to 50+ session chronicles spanning multiple continents.

**Have fun with it.** The kit's cross-pack institutional infrastructure exists to support chronicle-active play — not to constrain it. If your chronicle goes off-script, the kit is robust enough to accommodate. If your chronicle goes on-script, the kit supplies dramatic stakes spanning Pacific Rim, Atlantic, and Eurasian institutional architecture.

Welcome to V:tM V5 in SillyTavern.

---

## Document maintenance

This `how_to_play.md` reflects kit state as of 2026-05-23 (post-Chicago integration). Updates should be made when:
- New lorebooks are added to the kit
- New character cards or scenario packs are added
- SillyTavern feature changes affect kit functionality
- Restraint stance methodology refinements emerge
- New cross-pack institutional axes are documented in `kit_canon.md`
