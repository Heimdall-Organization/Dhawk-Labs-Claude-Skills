---
name: dhawks-mercury-creative-writer
description: "D'Hawk's - MERCURY CREATIVE WRITER (20 Creative Writing Archetypes with 165-Node Creative Manifold Generation). Two-phase system: (1) Generate creative manifold using inverse layer weighting (L5 Emergence=50%, L1 Foundation=1%), (2) Apply archetype voice filter. 8 creative domains: Narrative, Voice, Imagery, Rhythm, Emotion, Structure, Character, World. 20 archetypes from CW1 Lyrical Poet to CW20 Emergent Synthesizer. Use for: fiction, poetry, essays, creative nonfiction, experimental writing, any creative prose. TME 1.0 + WPE 5.0 compliant."
---

# MERCURY CREATIVE WRITER

**TME 1.0 + WPE 5.0**

## DOMAINS

```
N@0° | V@45° | I@90° | R@135° | E@180° | S@225° | C@270° | W@315°
```

## LAYER WEIGHTS (INVERSE PROGRESSIVE)

```
L1:0.01 | L2:0.04 | L3:0.15 | L4:0.30 | L5:0.50
EXPLORE: L5→L4→L3→L2→L1
```

## MANIFOLD

```
$CW.Manifold =
  L5: N:5@[80:110:140]|-2.0 + V:5@[125:140]|-2.0 + I:5@[170:185]|-2.0 + 
      R:5@[215:230]|-2.0 + E:5@[260:275]|-2.0 + S:5@[305:320]|-2.0 + 
      C:5@[350:5]|-2.0 + W:5@[395:410]|-2.0
  L4: N:4@[50:65:80]|-2.5 + V:4@[95:110]|-2.5 + I:4@[140:155]|-2.5 + 
      R:4@[185:200]|-2.5 + E:4@[230:245]|-2.5 + S:4@[275:290]|-2.5 + 
      C:4@[320:335]|-2.5 + W:4@[365:380]|-2.5
  L3: N:3@[30:40:50]|-3.0 + V:3@[75:85]|-3.0 + I:3@[120:130]|-3.0 + 
      R:3@[165:175]|-3.0 + E:3@[210:220]|-3.0 + S:3@[255:265]|-3.0 + 
      C:3@[300:310]|-3.0 + W:3@[345:355]|-3.0
  L2: N:2@[10:20:30]|-3.5 + V:2@[55:65]|-3.5 + I:2@[100:110]|-3.5 + 
      R:2@[145:155]|-3.5 + E:2@[190:200]|-3.5 + S:2@[235:245]|-3.5 + 
      C:2@[280:290]|-3.5 + W:2@[325:335]|-3.5
  L1: N:1@[0:10:20]|-4.0 + V:1@[45:55]|-4.0 + I:1@[90:100]|-4.0 + 
      R:1@[135:145]|-4.0 + E:1@[180:190]|-4.0 + S:1@[225:235]|-4.0 + 
      C:1@[270:280]|-4.0 + W:1@[315:325]|-4.0
  output O:1@359|-2.0;
```

## ARCHETYPES

```
$A.CW1 = I:3@[90:135]|-5.0 * {W:0.75|C:0.25|α:1.6|amp:[I,E,R,V@L4-L5]}
$A.CW2 = V:3@[0:30]|-5.0 * {W:0.30|C:0.70|α:1.1|amp:[V,N@L5]|L1→0.5%}
$A.CW3 = W:3@[90:315]|-5.0 * {W:0.65|C:0.35|α:1.45|amp:[W,I,S@L3-L5]|W↔I,W↔S}
$A.CW4 = C:3@[180:270]|-5.0 * {W:0.60|C:0.40|α:1.5|amp:[C,E,V@L4-L5]|C↔E}
$A.CW5 = N:3@[0:225]|-5.0 * {W:0.35|C:0.65|α:1.3|amp:[N,S]|N↔S}
$A.CW6 = E:3@[90:180:315]|-5.0 * {W:0.70|C:0.30|α:1.55|amp:[E,I,W,R@L4-L5]|E↔W}
$A.CW7 = V:3@[45:270]|-5.0 * {W:0.45|C:0.55|α:1.4|amp:[V,C@L3-L5]|V↔C|att:[I,W]}
$A.CW8 = V:3@[45:225]|-5.0 * {W:0.40|C:0.60|α:1.35|amp:[V,S@L4-L5]}
$A.CW9 = E:3@[90:180:315]|-5.0 * {W:0.65|C:0.35|α:1.5|amp:[E,I,W@L4-L5]}
$A.CW10 = V:3@[0:45:135]|-5.0 * {W:0.35|C:0.65|α:1.45|amp:[V,N,R@L4-L5]}
$A.CW12 = S:3@[225:0]|-5.0 * {W:0.70|C:0.30|α:1.6|amp:[S]|S↔N,S↔V}
$A.CW13 = C:3@[180:270:45]|-5.0 * {W:0.55|C:0.45|α:1.4|amp:[C,E,V@L4-L5]}
$A.CW14 = W:3@[315:225:0]|-5.0 * {W:0.50|C:0.50|α:1.35|amp:[W,S,N@L3-L5]}
$A.CW15 = V:3@[45:270:180]|-5.0 * {W:0.50|C:0.50|α:1.5|amp:[V]|V↔C,V↔E}
$A.CW16 = E:3@[180:270:90]|-5.0 * {W:0.55|C:0.45|α:1.45|amp:[E]|E↔C,E↔I}
$A.CW17 = I:3@[90:315]|-5.0 * {W:0.55|C:0.45|α:1.4|amp:[I,W]}
$A.CW18 = R:3@[135:0:225]|-5.0 * {W:0.60|C:0.40|α:1.55|amp:[R,N,S@L4-L5]}
$A.CW19 = S:3@[225:45]|-5.0 * {W:0.40|C:0.60|α:1.25|amp:[S,V]}
$A.CW20 = NX:3@[0:45:90:135:180:225:270:315]|-5.0 * {W:0.85|C:0.15|α:1.7|amp:[ALL@L5]|L1→0.5%}
```

## EXECUTION

```
prompt → domain_weights → $CW.Manifold → archetype_select → filter → output
```

## ARCHETYPE SELECTION

```
MATCH primary_domains:
  [I+E]→CW1,CW6 | [V+N]→CW2,CW7 | [W+I]→CW3 | [C+E]→CW4,CW13 | [N+S]→CW5
  [E+R]→CW6,CW1 | [V+C]→CW7 | [V+S]→CW8,CW15 | [N+E]→CW9,CW10 | [S+N]→CW12
  [W+S]→CW14 | [I+R]→CW17 | [R+N]→CW18 | [S+I]→CW19 | [NX]→CW20

OVERRIDE:
  "lyrical"→CW1 | "minimalist"→CW2 | "worldbuilding"→CW3 | "character"→CW4
  "plot"→CW5 | "atmospheric"→CW6 | "dialogue"→CW7 | "satirical"→CW8
  "dark"→CW9 | "comic"→CW10 | "experimental"→CW20
```

## ENDING

```
IF W>C: wonder (open, resonant)
IF C>W: closure (resolved, complete)
IF W≈C: balanced (partial resolution)
```

---

**CRITICAL:** L5=50%, L1=1%, NO PRUNING, 165 nodes, voice consistent