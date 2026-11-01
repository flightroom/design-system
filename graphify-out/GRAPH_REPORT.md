# Graph Report - design-system  (2026-11-01)

## Corpus Check
- 125 files · ~25,459 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 561 nodes · 1244 edges · 32 communities (21 shown, 11 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS · INFERRED: 2 edges (avg confidence: 0.72)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `8a759e7e`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- [[_COMMUNITY_Core UI Primitives|Core UI Primitives]]
- [[_COMMUNITY_Package Metadata|Package Metadata]]
- [[_COMMUNITY_Select Component|Select Component]]
- [[_COMMUNITY_Form System & RHF Fields|Form System & RHF Fields]]
- [[_COMMUNITY_TypeScript Config|TypeScript Config]]
- [[_COMMUNITY_Runtime Dependencies|Runtime Dependencies]]
- [[_COMMUNITY_Docs & CICD Pipeline|Docs & CI/CD Pipeline]]
- [[_COMMUNITY_Badge & Sidebar Navigation|Badge & Sidebar Navigation]]
- [[_COMMUNITY_Dialogs & Color Picker|Dialogs & Color Picker]]
- [[_COMMUNITY_Dev Dependencies|Dev Dependencies]]
- [[_COMMUNITY_Tabs Component|Tabs Component]]
- [[_COMMUNITY_Button & Calendar Field|Button & Calendar Field]]
- [[_COMMUNITY_Dropdown Menu|Dropdown Menu]]
- [[_COMMUNITY_Table Component|Table Component]]
- [[_COMMUNITY_Card Component|Card Component]]
- [[_COMMUNITY_CLAUDE|CLAUDE.md]]
- [[_COMMUNITY_Atoms (Button, Badge)|Atoms (Button, Badge)]]
- [[_COMMUNITY_class-variance-authority|class-variance-authority]]
- [[_COMMUNITY_Form Fields (TextField, SelectField, ...)|Form Fields (TextField, SelectField, ...)]]
- [[_COMMUNITY_MFE Orchestrator|MFE Orchestrator]]
- [[_COMMUNITY_Navigation Components (Sidebar, NavItem)|Navigation Components (Sidebar, NavItem)]]
- [[_COMMUNITY_Primitives (Accordion, Alert, Card, Dialog, ...)|Primitives (Accordion, Alert, Card, Dialog, ...)]]
- [[_COMMUNITY_Radix UI|Radix UI]]
- [[_COMMUNITY_react-hook-form|react-hook-form]]
- [[_COMMUNITY_Tailwind CSS v4|Tailwind CSS v4]]
- [[_COMMUNITY_theme.css Design Tokens|theme.css Design Tokens]]
- [[_COMMUNITY_IconTile.tsx|IconTile.tsx]]
- [[_COMMUNITY_NumberedSteps.tsx|NumberedSteps.tsx]]
- [[_COMMUNITY_graphify|graphify]]
- [[_COMMUNITY_SliderField.rhf.tsx|SliderField.rhf.tsx]]
- [[_COMMUNITY_Meter.tsx|Meter.tsx]]

## God Nodes (most connected - your core abstractions)
1. `cn()` - 94 edges
2. `getTestId()` - 90 edges
3. `TestIdProps` - 88 edges
4. `compilerOptions` - 20 edges
5. `formatter` - 13 edges
6. `correctness` - 12 edges
7. `Label` - 12 edges
8. `Button` - 11 edges
9. `@flightroom/design-system` - 11 edges
10. `formatter` - 10 edges

## Surprising Connections (you probably didn't know these)
- `LogViewerActions()` --references--> `url`  [EXTRACTED]
  src/components/ui/logViewer/LogViewerActions.tsx → package.json
- `SliderField()` --calls--> `getTestId()`  [EXTRACTED]
  src/components/input/SliderField.rhf.tsx → src/utils/testIdUtils.ts
- `DeleteConfirmationDialogProps` --inherits--> `TestIdProps`  [EXTRACTED]
  src/components/ui/DeleteConfirmationDialog.tsx → src/utils/testIdUtils.ts
- `EntityPickerList()` --calls--> `cn()`  [EXTRACTED]
  src/components/ui/entityPickerList/EntityPickerList.tsx → src/utils/styleUtils.ts
- `ISelectControlProps` --inherits--> `TestIdProps`  [EXTRACTED]
  src/components/ui/select/partials/selectControl/selectControl.tsx → src/utils/testIdUtils.ts

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Tag-triggered release to GitHub Packages** — _github_workflows_release_release_workflow, _github_workflows_release_publish_job, readme_github_packages, _github_workflows_release_tag_driven_versioning [EXTRACTED 1.00]

## Communities (32 total, 11 thin omitted)

### Community 0 - "Core UI Primitives"
Cohesion: 0.20
Nodes (9): Badge(), IBadgeProps, BadgeVariants, BadgeVariant, DOT_TONE, IStatusBadgeProps, IStatusDotProps, StatusDot() (+1 more)

### Community 1 - "Package Metadata"
Cohesion: 0.04
Nodes (46): description, devDependencies, @biomejs/biome, react, react-dom, react-hook-form, @types/node, @types/react (+38 more)

### Community 2 - "Select Component"
Cohesion: 0.05
Nodes (48): CalendarField(), CalendarFieldProps, Spinner(), SpinnerProps, Accordion, AccordionContent, AccordionItem, AccordionTrigger (+40 more)

### Community 3 - "Form System & RHF Fields"
Cohesion: 0.17
Nodes (17): Checkbox, fieldText(), ILogLineProps, JsonObject, levelClass(), levelOf(), LogLine(), LogViewerLine (+9 more)

### Community 4 - "TypeScript Config"
Cohesion: 0.05
Nodes (40): source, assist, actions, enabled, css, parser, files, ignoreUnknown (+32 more)

### Community 5 - "Runtime Dependencies"
Cohesion: 0.08
Nodes (24): dependencies, class-variance-authority, clsx, date-fns, lucide-react, @radix-ui/react-accordion, @radix-ui/react-avatar, @radix-ui/react-checkbox (+16 more)

### Community 6 - "Docs & CI/CD Pipeline"
Cohesion: 0.17
Nodes (11): Accessibilità, Contenuto, @flightroom/design-system, Installazione, License, Palette e token, Release, Setup Tailwind (v4) (+3 more)

### Community 7 - "Badge & Sidebar Navigation"
Cohesion: 0.15
Nodes (17): ColorSwatch(), IColorSwatchProps, colorSwatchVariants, DescriptionItem(), IDescriptionItemProps, DescriptionList(), DescriptionListContext, DescriptionListOrientation (+9 more)

### Community 8 - "Dialogs & Color Picker"
Cohesion: 0.11
Nodes (19): Button, spinnerSizeByButtonSize, ButtonVariants, IButtonProps, CopyButton, ICopyButtonProps, CodeBlock(), ICodeBlockProps (+11 more)

### Community 9 - "Dev Dependencies"
Cohesion: 0.07
Nodes (30): noArguments, noExtraBooleanCast, noUselessCatch, noUselessTypeConstraint, noConstantCondition, noConstAssign, noPrecisionLoss, noSelfAssign (+22 more)

### Community 10 - "Tabs Component"
Cohesion: 0.23
Nodes (8): NavItem, NavItemProps, navItemVariants, Sidebar, SidebarNavItemProps, SidebarProps, SidebarSlot, SidebarSlotState

### Community 11 - "Button & Calendar Field"
Cohesion: 0.08
Nodes (23): compilerOptions, allowSyntheticDefaultImports, declaration, declarationMap, emitDeclarationOnly, esModuleInterop, isolatedModules, jsx (+15 more)

### Community 12 - "Dropdown Menu"
Cohesion: 0.23
Nodes (7): TabsList, tabsListVariants, TabsTrigger, tabsTriggerVariants, Tabs, TabsContext, TabsProps

### Community 13 - "Table Component"
Cohesion: 0.09
Nodes (26): Alert, AlertDescription, alertVariants, ApiStatusQuery, IApiStatusHandlerProps, EmptyState(), EmptyStateTone, IEmptyStateProps (+18 more)

### Community 14 - "Card Component"
Cohesion: 0.18
Nodes (15): Card, CardContent, CardDescription, CardDivProps, CardFooter, CardHeader, CardTitle, DangerZoneCard() (+7 more)

### Community 18 - "CLAUDE.md"
Cohesion: 0.33
Nodes (6): Build Job, CI Workflow, Publish Job, Release Workflow, Tag-driven Version Alignment, GitHub Packages Registry

### Community 29 - "IconTile.tsx"
Cohesion: 0.24
Nodes (9): IconTile(), IconTileShape, IconTileSize, IconTileTone, IIconTileProps, iconTileVariants, AddTile, IAddTileProps (+1 more)

### Community 32 - "NumberedSteps.tsx"
Cohesion: 0.06
Nodes (50): ColorPicker(), ColorPickerCustomProps, DEFAULT_COLORS, SelectField(), SelectFieldProps, Switch(), SwitchCustomProps, TextareaChipsField() (+42 more)

### Community 37 - "SliderField.rhf.tsx"
Cohesion: 0.21
Nodes (9): SliderField(), SliderFieldProps, Slider, SliderProps, ToggleGroup, ToggleGroupContext, ToggleGroupItem, Toggle (+1 more)

### Community 41 - "Meter.tsx"
Cohesion: 0.57
Nodes (4): IMeterProps, Meter(), meterFillVariants, meterTrackVariants

## Knowledge Gaps
- **233 isolated node(s):** `$schema`, `enabled`, `clientKind`, `useIgnoreFile`, `ignoreUnknown` (+228 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **11 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `cn()` connect `Select Component` to `Core UI Primitives`, `NumberedSteps.tsx`, `Form System & RHF Fields`, `SliderField.rhf.tsx`, `Badge & Sidebar Navigation`, `Dialogs & Color Picker`, `Meter.tsx`, `Tabs Component`, `Dropdown Menu`, `Table Component`, `Card Component`, `IconTile.tsx`?**
  _High betweenness centrality (0.245) - this node is a cross-community bridge._
- **Why does `LogViewerActions()` connect `Form System & RHF Fields` to `Package Metadata`, `Select Component`?**
  _High betweenness centrality (0.165) - this node is a cross-community bridge._
- **Why does `url` connect `Package Metadata` to `Form System & RHF Fields`?**
  _High betweenness centrality (0.162) - this node is a cross-community bridge._
- **What connects `$schema`, `enabled`, `clientKind` to the rest of the system?**
  _234 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Package Metadata` be split into smaller, more focused modules?**
  _Cohesion score 0.043478260869565216 - nodes in this community are weakly interconnected._
- **Should `Select Component` be split into smaller, more focused modules?**
  _Cohesion score 0.05146242132543503 - nodes in this community are weakly interconnected._
- **Should `TypeScript Config` be split into smaller, more focused modules?**
  _Cohesion score 0.0524390243902439 - nodes in this community are weakly interconnected._