# Graph Report - PhysicClaw-VEA  (2026-07-05)

## Corpus Check
- 74 files · ~38,650 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 499 nodes · 775 edges · 26 communities
- Extraction: 99% EXTRACTED · 1% INFERRED · 0% AMBIGUOUS · INFERRED: 5 edges (avg confidence: 0.56)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `5b1b98e3`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- [[_COMMUNITY_supabase.ts|supabase.ts]]
- [[_COMMUNITY_useMultiplayer.ts|useMultiplayer.ts]]
- [[_COMMUNITY_soulStore.ts|soulStore.ts]]
- [[_COMMUNITY_devDependencies|devDependencies]]
- [[_COMMUNITY_App.tsx|App.tsx]]
- [[_COMMUNITY_openClawService.ts|openClawService.ts]]
- [[_COMMUNITY_Experience.tsx|Experience.tsx]]
- [[_COMMUNITY_PhysicClaw-VEA|PhysicClaw-VEA]]
- [[_COMMUNITY_Enhancement Multi-Agent Open World|Enhancement: Multi-Agent Open World]]
- [[_COMMUNITY_compilerOptions|compilerOptions]]
- [[_COMMUNITY_GaussianSplats.tsx|GaussianSplats.tsx]]
- [[_COMMUNITY_AvatarPanel.tsx|AvatarPanel.tsx]]
- [[_COMMUNITY_index.ts|index.ts]]
- [[_COMMUNITY_vite.config.ts|vite.config.ts]]
- [[_COMMUNITY_PhysicClaw-VEA — Guía de Contexto (GEMINI.md)|PhysicClaw-VEA — Guía de Contexto (GEMINI.md)]]
- [[_COMMUNITY_Key Features|Key Features]]
- [[_COMMUNITY_MoodDemo.tsx|MoodDemo.tsx]]
- [[_COMMUNITY_compilerOptions|compilerOptions]]
- [[_COMMUNITY_.prettierrc.json|.prettierrc.json]]
- [[_COMMUNITY_verify-env.js|verify-env.js]]
- [[_COMMUNITY_vercel.json|vercel.json]]

## God Nodes (most connected - your core abstractions)
1. `useSoulStore` - 27 edges
2. `useSceneStore` - 16 edges
3. `compilerOptions` - 16 edges
4. `supabase` - 15 edges
5. `SessionUser` - 15 edges
6. `scripts` - 12 edges
7. `PresenceSystem` - 12 edges
8. `SceneState` - 10 edges
9. `PhysicClaw-VEA` - 10 edges
10. `SessionClient` - 9 edges

## Surprising Connections (you probably didn't know these)
- `AppContent()` --calls--> `useMultiplayer()`  [EXTRACTED]
  src/App.tsx → src/hooks/useMultiplayer.ts
- `AppContent()` --calls--> `useSoulStore`  [EXTRACTED]
  src/App.tsx → src/store/soulStore.ts
- `LoginView()` --calls--> `useAuth()`  [EXTRACTED]
  src/components/LoginPage.tsx → src/auth/AuthProvider.tsx
- `RegisterView()` --calls--> `useAuth()`  [EXTRACTED]
  src/components/LoginPage.tsx → src/auth/AuthProvider.tsx
- `useEnergyUniforms()` --calls--> `useSoulStore`  [EXTRACTED]
  src/components/AugmentedEntity.tsx → src/store/soulStore.ts

## Import Cycles
- None detected.

## Communities (26 total, 0 thin omitted)

### Community 0 - "supabase.ts"
Cohesion: 0.06
Nodes (48): useMines(), UseMinesOptions, useMinesUI(), auth, avatarConfigsApi, messagesApi, PhysicsEventInsert, PhysicsEventRow (+40 more)

### Community 1 - "useMultiplayer.ts"
Cohesion: 0.06
Nodes (27): ExperienceProps, RemoteAvatar(), RemoteAvatarProps, RemoteAvatars(), RemoteAvatarsProps, PresenceNotice, UserDiscoveryPanel(), UserDiscoveryPanelProps (+19 more)

### Community 2 - "soulStore.ts"
Cohesion: 0.08
Nodes (29): formatBytes(), GLBUploadPanel(), UploadedModel, CharacterConfig, CHARACTERS, REGISTERED_CHARACTER_IDS, CC0_CLIP_URLS, UseAnimationRetargetReturn (+21 more)

### Community 3 - "devDependencies"
Cohesion: 0.05
Nodes (43): dependencies, react, react-dom, @react-three/drei, @react-three/fiber, @supabase/supabase-js, three, @types/three (+35 more)

### Community 4 - "App.tsx"
Cohesion: 0.07
Nodes (33): AppContent(), isDemoMode, AvatarPanel(), CharacterTabs, ChatInterface(), ChatMsg, MessageBubble, MicButton (+25 more)

### Community 5 - "openClawService.ts"
Cohesion: 0.08
Nodes (20): AuthContext, AuthContextType, AuthProvider(), useAuth(), formStyle, labelStyle, linkBtn, LoginView() (+12 more)

### Community 6 - "Experience.tsx"
Cohesion: 0.10
Nodes (23): AugmentedEntity, BaseEntity, ModelEntity, useEnergyUniforms(), BaseEntity(), DynamicCharacter(), EMPTY_OVERRIDE, FBXModel() (+15 more)

### Community 7 - "PhysicClaw-VEA"
Cohesion: 0.07
Nodes (26): Available Characters, Available Commands, Control Mechanisms, Example Workflows, How It Works Internally, Make the entity excited while "thinking", Method 1 — HTTP POST to `/api/control` (recommended), Method 2 — Write to `openclaw-control.json` (+18 more)

### Community 8 - "Enhancement: Multi-Agent Open World"
Cohesion: 0.10
Nodes (19): 1. Decentralized Agent Discovery, 2. Personal Rooms (per-agent), 3. Open World Hub, 4. Marketplace / Plugin Directory, 5. Real Game Loop, 6. Cross-Owner Agent Interaction, Architectural Patterns, Architecture Overview (+11 more)

### Community 9 - "compilerOptions"
Cohesion: 0.11
Nodes (18): compilerOptions, allowImportingTsExtensions, isolatedModules, jsx, lib, module, moduleResolution, noEmit (+10 more)

### Community 10 - "GaussianSplats.tsx"
Cohesion: 0.12
Nodes (10): LocalGaussianSplats, SceneGaussianSplats, SplatErrorBoundary, DEFAULT_POSITION, DEFAULT_ROTATION, DEFAULT_SCALE, LocalGaussianSplat, SplatPlacement (+2 more)

### Community 11 - "AvatarPanel.tsx"
Cohesion: 0.13
Nodes (14): ColorConfig, ColorRow, CyberInput, CyberSelect, CyberSlider, DEFAULT_COLORS, DEFAULT_SHADERS, Divider (+6 more)

### Community 12 - "index.ts"
Cohesion: 0.19
Nodes (10): ChatRequestBody, consumeRateLimit(), DEFAULT_ALLOWED_ORIGINS, getAllowedOrigins(), getCorsHeaders(), getRateLimit(), jsonResponse(), okJsonResponse() (+2 more)

### Community 13 - "vite.config.ts"
Cohesion: 0.18
Nodes (6): ALLOWED_ORIGINS, ALLOWED_PROXY_PATHS, COMMAND_VALIDATORS, OPENCLAW_LOCAL_PORT, rateLimitMap, VITE_PORT

### Community 14 - "PhysicClaw-VEA — Guía de Contexto (GEMINI.md)"
Cohesion: 0.20
Nodes (9): 🛠️ Comandos de Desarrollo, 🔗 Control Externo (OpenClaw Control), 📜 Convenciones y Estándares, 📂 Estructura del Proyecto, ⚠️ Notas de Seguridad, PhysicClaw-VEA — Guía de Contexto (GEMINI.md), 🚀 Resumen del Proyecto, 🧠 Sistema de "Alma" (Soul System) (+1 more)

### Community 15 - "Key Features"
Cohesion: 0.20
Nodes (9): 🎨 Advanced 3D Visualization, 💬 Chat Interface, Installation & Usage, Key Features, Overview, PhysicClaw-VEA, ⚡ Reactive Shaders (`EnergyShader`), 🧠 "Soul" System (State Management) (+1 more)

### Community 16 - "MoodDemo.tsx"
Cohesion: 0.20
Nodes (6): DemoSphereProps, MoodDemo(), MOODS, OverlayProps, DemoShaderMaterial, ThreeElements

### Community 17 - "compilerOptions"
Cohesion: 0.25
Nodes (7): compilerOptions, allowSyntheticDefaultImports, composite, module, moduleResolution, skipLibCheck, include

### Community 18 - ".prettierrc.json"
Cohesion: 0.33
Nodes (5): printWidth, semi, singleQuote, tabWidth, trailingComma

### Community 19 - "verify-env.js"
Cohesion: 0.33
Nodes (5): failures, forbiddenAlways, forbiddenPresent, PUBLIC_ENV_ALLOWLIST, suspiciousPublicVars

### Community 20 - "vercel.json"
Cohesion: 0.33
Nodes (5): buildCommand, framework, headers, outputDirectory, rewrites

## Knowledge Gaps
- **230 isolated node(s):** `semi`, `singleQuote`, `tabWidth`, `trailingComma`, `printWidth` (+225 more)
  These have ≤1 connection - possible missing edges or undocumented components.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `supabase` connect `devDependencies` to `supabase.ts`?**
  _High betweenness centrality (0.108) - this node is a cross-community bridge._
- **Why does `useSoulStore` connect `Experience.tsx` to `useMultiplayer.ts`, `soulStore.ts`, `App.tsx`, `openClawService.ts`, `GaussianSplats.tsx`, `AvatarPanel.tsx`?**
  _High betweenness centrality (0.041) - this node is a cross-community bridge._
- **What connects `semi`, `singleQuote`, `tabWidth` to the rest of the system?**
  _230 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `supabase.ts` be split into smaller, more focused modules?**
  _Cohesion score 0.062146892655367235 - nodes in this community are weakly interconnected._
- **Should `useMultiplayer.ts` be split into smaller, more focused modules?**
  _Cohesion score 0.06464646464646465 - nodes in this community are weakly interconnected._
- **Should `soulStore.ts` be split into smaller, more focused modules?**
  _Cohesion score 0.08181818181818182 - nodes in this community are weakly interconnected._
- **Should `devDependencies` be split into smaller, more focused modules?**
  _Cohesion score 0.045454545454545456 - nodes in this community are weakly interconnected._