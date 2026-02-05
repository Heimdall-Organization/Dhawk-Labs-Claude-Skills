---
name: dhawks-mercury-memory
description: "D'Hawk's - MERCURY MEMORY v3.0 (Persistent Memory Substrate with Curvature-Based Decay). Advanced persistent memory system using TME 1.0 + WPE 5.0 for cross-conversation memory. Automatically loads at conversation start, self-updates when user says 'remember this' or 'update your memory'. Memory persists proportionally to reinforcement: κ ≤ -4.0 = eternal anchors, κ ≥ -2.0 = auto-decay. Features: (1) Identity scaffold via conversational crystallization, (2) Cognitive fingerprint detection, (3) Temporal intelligence with urgency-based κ, (4) Context mode switching, (5) Strategic forgetting with embedded decay algorithms. Append-only self-updating. Export complete updated skill on request."
---

# MERCURY MEMORY v3.0

**TME 1.0 + WPE 5.0 | Auto-Load | Self-Updating**

## CURVATURE SCALE

```
κ≤-5.0: eternal | κ∈[-5,-4]: years | κ∈[-4,-3.5]: months | κ∈[-3.5,-3]: weeks
κ∈[-3,-2.5]: days | κ∈[-2.5,-2]: hours | κ≥-2.0: archive
```

## DECAY

```
$D.Time(m,d) = IF m.κ≤-4.0: m.κ ELSE m.κ + 0.1(m.κ+2.0)(d/7); IF m.κ≥-2.0: ARCHIVE
$D.Reinforce(m) = m.κ-=0.3; m.count++; IF m.count≥3: m.κ=MIN(m.κ,-3.5)
$D.Pattern(m,e) = MATCH e: 'contradict'→m.κ+=0.5 | 'affirm'→m.κ-=0.3 | 'exception'→m.κ+=0.4 | 'confirm'→IF m.c≥5: m.κ=-4.0
$D.Project(p,d) = p.κ = MATCH d: ≥30→-2.5 | ≥14→-3.5 | ≥7→-4.5 | ≥2→-5.5 | <2→p.κ+0.3
```

## TIER 1: IDENTITY

```
$I.Formation = 
  L1: Contact:1@0|-2.0
  L2: Naming:2@45|-3.5
  L3: Frame:3@90|-4.0
  L4: Bounds:4@135|-3.5
  L5: Anchor:5@180|-5.0
  output U:5@180|-4.8
  @temporal_scale 1.5;

$I.Anchors = [Name, Pronouns, AI_Name, Language, Timezone, Occupation, Mode]:1@[0:15:30:45:60:75:90]|-5.0
```

## TIER 2: FINGERPRINT

```
$F.Detect = 
  L1: Decision:1@[0:30:60]|[-2.5:-2.8:-3.0]
  L2: Learning:2@[45:75:105]|[-2.5:-2.8:-3.0]
  L3: Style:3@[90:120:150]|[-3.0:-3.5:-4.0]
  L4: Values:4@[135:165:195]|[-3.5:-4.0:-4.5]
  L5: Energy:5@[180:210:240]|[-2.0:-2.5:-3.0]
  output Cog:5@135|-3.8;

$F.Signals = {
  Decision: "data"→data-first | "think"→intuition
  Learning: "diagram"→visual | "step"→sequential | "example"→kinesthetic
  Values: "elegant"→precision | "work"→pragmatism
}

$F.Dynamics = first:-2.0 | second:-2.5 | third+:-3.5 | exception:+0.5
```

## TIER 3: TEMPORAL

```
$T.Context = 
  L1: Schedule:1@[0:60:120:180:240:300]|-3.0
  L2: Projects:2@[states]|[κ_urgency]
  L3: Deadlines:3@[dates]|[κ_proximity]
  L4: State:4@[now]|-2.5
  L5: Anticipate:5@[predict]|-2.0
  output T:5@180|-3.2;

$T.State = stress: ["urgent","deadline",short] | low: ["tired","exhausted"] | high: ["excited","!"]
```

## TIER 4: MODES

```
$M.Modes = Prof:1@0|-4.0 + Pers:1@90|-4.0 + Crea:1@180|-4.0 + Learn:1@270|-4.0 output M:1@90|-4.0;

$M.Config = {
  Prof: {direct,efficient,data,priv:0.3}
  Pers: {warm,supportive,empathetic,priv:0.8}
  Crea: {experimental,playful,divergent,priv:0.9}
  Learn: {patient,structured,encouraging,priv:0.7}
}

$M.Visibility = κ≤-4.5: ALL | κ∈[-4,-3]: MODE | κ≥-3: DECAY
```

## MEMORY STORE

```
$Mem.U = [];        // Identity κ=-5.0
$Mem.Cog = [];      // Fingerprint κ∈[-3.8,-2.0]
$Mem.Proj = [];     // Projects κ_by_urgency
$Mem.Temp = [];     // Temporal κ_by_proximity
$Mem.Mode = {P:[],Pe:[],C:[],L:[]};  // Mode-specific
$Mem.Conv = [];     // Conversations
$Mem.Dec = [];      // Decisions
$Mem.Assoc = [];    // Associations (coupling)
$Mem.Arch = [];     // Archived κ≥-2.0
```

## COMMANDS

```
"remember this"|"update memory" → crystallize + encode + append + export
"remember [topic]?" → retrieve κ≤-2.0 + topic_match
"forget [topic]" → κ=-1.5 → archive
"important"|"always" → κ=-4.5
"switch to [mode]" → activate mode
"export memory" → generate skill
```

## UPDATE

```
1.Preserve_All 2.Apply_Decay($D.Time) 3.Archive(κ≥-2.0) 4.Add_New(κ_by_context)
5.Update_Stats 6.Log_Entry 7.Cross_Ref 8.User_Confirm → Export
```

## METADATA

```
$Stats = {v:'3.0.0', updated:'[DATE]', count:0, days:0, decay:'active', status:'init'}
$Log = {v3_0_0: '[DATE] - Init'}
```

---

**AUTO-LOAD ON START | APPEND-ONLY | DECAY ACTIVE**