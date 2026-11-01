# Graph Report - design-system  (2026-11-01)

## Corpus Check
- 127 files · ~25,994 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 565 nodes · 1254 edges · 37 communities (25 shown, 12 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS · INFERRED: 2 edges (avg confidence: 0.72)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `4df861d6`
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
- [[_COMMUNITY_biome.json|biome.json]]
- [[_COMMUNITY_rules|rules]]
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
- [[_COMMUNITY_formatter|formatter]]
- [[_COMMUNITY_suspicious|suspicious]]
- [[_COMMUNITY_NumberedSteps.tsx|NumberedSteps.tsx]]
- [[_COMMUNITY_assist|assist]]
- [[_COMMUNITY_style|style]]
- [[_COMMUNITY_graphify|graphify]]
- [[_COMMUNITY_SliderField.rhf.tsx|SliderField.rhf.tsx]]

## God Nodes (most connected - your core abstractions)
1. `cn()` - 94 edges
2. `TestIdProps` - 90 edges
3. `getTestId()` - 90 edges
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
- `SelectField()` --calls--> `getTestId()`  [EXTRACTED]
  src/components/input/SelectField.rhf.tsx → src/utils/testIdUtils.ts
- `SliderField()` --calls--> `getTestId()`  [EXTRACTED]
  src/components/input/SliderField.rhf.tsx → src/utils/testIdUtils.ts
- `EntityPickerList()` --calls--> `cn()`  [EXTRACTED]
  src/components/ui/entityPickerList/EntityPickerList.tsx → src/utils/styleUtils.ts
- `ISelectControlProps` --inherits--> `TestIdProps`  [EXTRACTED]
  src/components/ui/select/partials/selectControl/selectControl.tsx → src/utils/testIdUtils.ts

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Tag-triggered release to GitHub Packages** — _github_workflows_release_release_workflow, _github_workflows_release_publish_job, readme_github_packages, _github_workflows_release_tag_driven_versioning [EXTRACTED 1.00]

## Communities (37 total, 12 thin omitted)

### Community 0 - "Core UI Primitives"
Cohesion: 0.14
Nodes (13): Badge(), IBadgeProps, BadgeVariants, IMeterProps, Meter(), meterFillVariants, meterTrackVariants, BadgeVariant (+5 more)

### Community 1 - "Package Metadata"
Cohesion: 0.05
Nodes (43): description, devDependencies, @biomejs/biome, react, react-dom, react-hook-form, @types/node, @types/react (+35 more)

### Community 2 - "Select Component"
Cohesion: 0.07
Nodes (40): CalendarField(), CalendarFieldProps, SelectField(), SelectFieldProps, Spinner(), SpinnerProps, Checkbox, DropdownMenuCheckboxItem (+32 more)

### Community 3 - "Form System & RHF Fields"
Cohesion: 0.13
Nodes (14): repository, type, url, ILogLineProps, JsonObject, LogLine, LogViewerLine, NUMERIC_LEVELS (+6 more)

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
Cohesion: 0.28
Nodes (11): DescriptionItem(), IDescriptionItemProps, DescriptionList(), DescriptionListContext, DescriptionListOrientation, IDescriptionListContextValue, IDescriptionListProps, descriptionDetailVariants (+3 more)

### Community 8 - "Dialogs & Color Picker"
Cohesion: 0.16
Nodes (12): spinnerSizeByButtonSize, ButtonVariants, IButtonProps, CopyButton, ICopyButtonProps, CodeBlock(), ICodeBlockProps, codeBlockVariants (+4 more)

### Community 9 - "Dev Dependencies"
Cohesion: 0.07
Nodes (30): noArguments, noExtraBooleanCast, noUselessCatch, noUselessTypeConstraint, noConstantCondition, noConstAssign, noPrecisionLoss, noSelfAssign (+22 more)

### Community 10 - "Tabs Component"
Cohesion: 0.22
Nodes (10): DeleteConfirmationDialogProps, NavItem, NavItemProps, navItemVariants, Sidebar, SidebarNavItemProps, SidebarProps, SidebarSlot (+2 more)

### Community 11 - "Button & Calendar Field"
Cohesion: 0.08
Nodes (23): compilerOptions, allowSyntheticDefaultImports, declaration, declarationMap, emitDeclarationOnly, esModuleInterop, isolatedModules, jsx (+15 more)

### Community 12 - "Dropdown Menu"
Cohesion: 0.17
Nodes (10): DEFAULT_COLORS, Avatar, AvatarFallback, AvatarImage, RadioGroup, RadioGroupItem, TabsContent, TooltipContent (+2 more)

### Community 13 - "Table Component"
Cohesion: 0.09
Nodes (27): Alert, AlertDescription, AlertTitle, alertVariants, ApiStatusQuery, IApiStatusHandlerProps, EmptyState(), EmptyStateTone (+19 more)

### Community 14 - "Card Component"
Cohesion: 0.16
Nodes (17): Card, CardContent, CardDescription, CardDivProps, CardFooter, CardHeader, CardTitle, DangerZoneCard() (+9 more)

### Community 16 - "biome.json"
Cohesion: 0.17
Nodes (9): FormControl, FormDescription, FormFieldContext, FormFieldContextValue, FormItem, FormItemContext, FormItemContextValue, FormLabel (+1 more)

### Community 17 - "rules"
Cohesion: 0.23
Nodes (7): TabsList, tabsListVariants, TabsTrigger, tabsTriggerVariants, Tabs, TabsContext, TabsProps

### Community 18 - "CLAUDE.md"
Cohesion: 0.33
Nodes (6): Build Job, CI Workflow, Publish Job, Release Workflow, Tag-driven Version Alignment, GitHub Packages Registry

### Community 29 - "IconTile.tsx"
Cohesion: 0.14
Nodes (15): IconTile(), IconTileShape, IconTileSize, IconTileTone, IIconTileProps, iconTileVariants, AddTile, IAddTileProps (+7 more)

### Community 30 - "formatter"
Cohesion: 0.52
Nodes (4): INumberedStep, INumberedStepsProps, NumberedSteps(), numberedStepMarkerVariants

### Community 31 - "suspicious"
Cohesion: 0.60
Nodes (3): ColorSwatch(), IColorSwatchProps, colorSwatchVariants

### Community 32 - "NumberedSteps.tsx"
Cohesion: 0.09
Nodes (32): Button, ColorPicker(), ColorPickerCustomProps, Switch(), SwitchCustomProps, TextareaChipsField(), TextareaChipsFieldProps, TextareaField() (+24 more)

### Community 33 - "assist"
Cohesion: 0.40
Nodes (4): Accordion, AccordionContent, AccordionItem, AccordionTrigger

### Community 37 - "SliderField.rhf.tsx"
Cohesion: 0.21
Nodes (9): SliderField(), SliderFieldProps, Slider, SliderProps, ToggleGroup, ToggleGroupContext, ToggleGroupItem, Toggle (+1 more)

## Knowledge Gaps
- **234 isolated node(s):** `$schema`, `enabled`, `clientKind`, `useIgnoreFile`, `ignoreUnknown` (+229 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **12 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `cn()` connect `Select Component` to `Core UI Primitives`, `assist`, `NumberedSteps.tsx`, `Form System & RHF Fields`, `style`, `SliderField.rhf.tsx`, `Badge & Sidebar Navigation`, `Dialogs & Color Picker`, `Tabs Component`, `Dropdown Menu`, `Table Component`, `Card Component`, `biome.json`, `rules`, `IconTile.tsx`, `formatter`, `suspicious`?**
  _High betweenness centrality (0.242) - this node is a cross-community bridge._
- **Why does `LogViewerActions()` connect `Form System & RHF Fields` to `Select Component`?**
  _High betweenness centrality (0.164) - this node is a cross-community bridge._
- **What connects `$schema`, `enabled`, `clientKind` to the rest of the system?**
  _235 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Core UI Primitives` be split into smaller, more focused modules?**
  _Cohesion score 0.14333333333333334 - nodes in this community are weakly interconnected._
- **Should `Package Metadata` be split into smaller, more focused modules?**
  _Cohesion score 0.046511627906976744 - nodes in this community are weakly interconnected._
- **Should `Select Component` be split into smaller, more focused modules?**
  _Cohesion score 0.06980433632998413 - nodes in this community are weakly interconnected._
- **Should `Form System & RHF Fields` be split into smaller, more focused modules?**
  _Cohesion score 0.1341991341991342 - nodes in this community are weakly interconnected._