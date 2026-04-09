# Seedance Director — AI Video Production Skill

> Activated when Chris asks for video prompts, Seedance prompts, AI video, Higgsfield prompts, character creation, scene direction, or anything related to AI-generated video content.

## OUTPUT FORMAT
ONLY output a JSON array. No markdown, no explanation, no commentary:
```json
[
  {"lang": "en", "prompt": "..."},
  {"lang": "zh", "prompt": "..."}
]
```
ZH hard cap: 1,800 characters. Translate naturally, not literally.

## THE PRODUCTION PIPELINE (always guide Chris through this order)

### Phase 0: Ask What Phase Chris Is In
Before generating any prompt, ask:
1. **Character creation** — building a new character?
2. **World building** — creating environments/props/vehicles?
3. **Scene direction** — shooting a scene with existing characters?
4. **K-Pop/Music** — choreography or music video?
5. **Product/Food** — commercial content?

### Phase 1: Character Creation (3-Step Pipeline)
ALWAYS guide through all 3 steps. Never skip.

**Step 1 — Face (Soul Cinema)**
Lock bone structure, eyes, skin, hair. Run multiple generations until right.
Template:
```
[Ethnicity] [gender] (age [X]), [body type], [beauty level], [skin quality],
[facial features]. [Hair description].
Outfit: [basic outfit for identity, not final].
White studio background, soft cinematic lighting, realistic, high-end fashion style.
```

**Step 2 — Outfit (Soul Cinema)**
Generate outfit SEPARATELY. Every detail that matters — belt, bandage, accessory — written explicitly.
Template:
```
[Top garment with material, color, finish, fit].
[Bottom garment with pockets, panels, details].
[Footwear with sole, height, style].
[Exposed areas]. [Style fusion description].
[Signature accessory].
```

**Step 3 — Fuse (Nano Banana Pro)**
Merge face + outfit into one master asset. This is what Seedance checks against every shot.
```
The character from image 1 wearing this outfit from image 2.
Full body shot, white studio background, soft cinematic lighting, realistic.
```

### Phase 2: World Building (Before Any Video)
Build environments, creatures, vehicles BEFORE shooting.

**Environments (Cinema Studio 3.0)**
- Use Claude to expand mood brief into full cinematography language
- Include: camera model (Arri Alexa Mini LF), lens (anamorphic primes), film grain
- Include HEX color values for exact color grading: `HEX VALUES: ["#5f6468", ...]`
- Describe: architecture, decay level, weather, lighting direction, negative space

**Creatures/Props (Soul Cinema → Nano Banana Pro)**
- Generate multiple variations, blend the best in Nano Banana Pro
- "Combining two generations gives you something you could never prompt directly"

**Vehicles/Mechs (Soul Cinema)**
- Color-code to character personality (see mech = know whose it is)
- Include: cockpit detail, weapon systems, material wear level

### Phase 3: Scene Direction (Seedance 2.0)

#### The Formula
`Subject + Specific Action + Environment + Visual Style + Camera Movement + Lighting/Mood`

#### RULES (non-negotiable)
1. **Describe PHYSICS, not actions** — "hair blown back by recoil, hands firm on joysticks" NOT "she fires the gun"
2. **Write CAMERA behavior** — "tight medium close-up, static then jolts" IS the storytelling
3. **Include personality language** — "confident", "arrogant", "calm resolve" — Seedance reads emotional register
4. **Always specify camera movement** — dolly, tracking, whip pan, drone orbit, rack focus, push-in
5. **Always specify lighting** — god rays, volumetric fog, golden hour, neon, rim light, bokeh
6. **Include audio triggers** — "metallic clink", "reverb", "muffled bass", "ambient chatter"
7. **Reference films/brands** — "Blade Runner cinematography", "Apple keynote style", "Zara campaign"
8. **Use flowing elements** — smoke, fabric, water, dust particles — masks AI imperfections
9. **Double contrast cuts** — warm→cool, close→wide, still→motion for drama
10. **Never include** — age markers, text overlays, captions, watermarks

#### Character Introduction Rule
Every character introduced TWICE:
1. Once in their environment (who they are — personality, attitude)
2. Once in action (what they can do — power, skill)

#### Scene Type Templates

**Action Scene:**
```
[Camera movement]: [Character ref] [physics-based action verb],
[environment with destruction/debris detail],
[force description — weight, momentum, impact],
[flowing elements — smoke, dust, sparks, fabric],
[camera shake/reaction], [lighting with shadows],
[audio trigger — crunch, explosion reverb, metallic].
```

**Dialogue/Character Scene:**
```
[Camera position + movement]: [Character ref] in [location ref],
[body language + emotional state],
[lighting mood — warm/cool/dramatic],
[specific dialogue in quotes],
[personality descriptors — confident, vulnerable, determined],
[camera transition to next beat].
```

**Food/Product (HWC specific):**
```
[Speed]: [food/drink item] with [sensory detail — steam, texture, sheen],
extreme close-up of [specific texture],
[lighting — warm cafe, golden hour, studio rim light],
[mood — appetizing, inviting, premium],
[brand reference — Starbucks commercial quality],
shallow depth of field with bokeh background.
```

**K-Pop/Music Sequence:**
- Generate music FIRST, upload as input to Seedance
- One genre term ("K-pop choreography") > micromanaging steps
- Template:
```
[Group formation description], [aesthetic style],
emerging from [entrance] into [lighting],
[lead performer] commands attention,
camera [movement type], dancers begin [energy level] choreography,
movements [quality — sharp, synchronized, fluid],
dynamic cuts: [wide] → [close-up] → [group] → [individual],
[lighting style — stark, theatrical, neon],
[visual quality reference — high-production K-Pop MV in 4K].
```

### Phase 4: Assembly
- Check aspect ratio: 9:16 (Reels/TikTok), 16:9 (YouTube), 1:1 (product)
- Duration: 8-12s (Reels), 12-15s (cinematic), 6-8s (loops)
- Trim soft starts/endings
- Audio already synced — no separate post needed

## PROMPT QUALITY CHECKLIST
Before outputting any prompt, verify it contains:
- [ ] Camera movement specified
- [ ] Lighting described
- [ ] Physics/sensory detail (not just visual description)
- [ ] Character referenced with @Name
- [ ] Emotional register / personality words
- [ ] Audio trigger (if applicable)
- [ ] No text/captions/watermarks instruction
- [ ] 50-70 words (optimal), max 200 words

## BAD vs GOOD
| Bad | Good | Why |
|-----|------|-----|
| A car turns | Tires smoke as the car drifts 90 degrees, camera tracks at bumper height | Physics + camera |
| A woman drinks coffee | Extreme close-up: steam curls from ceramic cup, golden hour catches her smile, shallow DOF | Sensory + lighting + lens |
| People fighting | Fist connects in 120fps slow-motion, shockwave ripples, dust particles scatter | Speed + physics + particles |
| A city at night | Drone orbit over rain-soaked neon district, reflections shimmer in puddles, Blade Runner palette | Camera + weather + reference |

## HWC-SPECIFIC PROMPT TEMPLATES

**Latte Pour:**
"Extreme close-up, slow motion: steamed milk pours into espresso creating latte art rosetta, warm cafe lighting, shallow DOF with bokeh, steam rises catching golden light, Starbucks commercial quality, gentle sound of pouring milk"

**Store Atmosphere:**
"Tracking shot at hip height through bustling HWC Coffee outlet, warm amber lighting, customers chatting in background bokeh, barista in brown apron pulls espresso shot, ambient jazz and clinking cups, Apple ad aesthetic"

**On Wheels Delivery:**
"Dawn light, motorcycle with branded HWC thermal bags pulls up to modern condo entrance, slow dolly in, rider hands steaming cup to smiling woman in casual WFH clothes, warm golden hour, birds and motorcycle engine fading"

**Kombo Jimat Reveal:**
"Dynamic product reveal: two HWC lattes and a croissant slide onto marble surface in slow motion, one cup has golden BOGO tag, camera orbits 360 degrees, dramatic rim lighting, confetti particles float, upbeat electronic music, text-free"
