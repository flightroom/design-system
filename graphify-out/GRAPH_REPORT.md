# Graph Report - design-system  (2026-11-01)

## Corpus Check
- 130 files · ~26,538 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 577 nodes · 1291 edges · 33 communities (22 shown, 11 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS · INFERRED: 2 edges (avg confidence: 0.72)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `4089b173`
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
- [[_COMMUNITY_NumberedSteps.tsx|NumberedSteps.tsx]]
- [[_COMMUNITY_graphify|graphify]]

## God Nodes (most connected - your core abstractions)
1. `cn()` - 96 edges
2. `TestIdProps` - 92 edges
3. `getTestId()` - 90 edges
4. `compilerOptions` - 20 edges
5. `formatter` - 13 edges
6. `correctness` - 12 edges
7. `Button` - 12 edges
8. `Label` - 12 edges
9. `@flightroom/design-system` - 11 edges
10. `formatter` - 10 edges

## Surprising Connections (you probably didn't know these)
- `LogViewerActions()` --references--> `url`  [EXTRACTED]
  src/components/ui/logViewer/LogViewerActions.tsx → package.json
- `SelectField()` --calls--> `getTestId()`  [EXTRACTED]
  src/components/input/SelectField.rhf.tsx → src/utils/testIdUtils.ts
- `TextField()` --calls--> `getTestId()`  [EXTRACTED]
  src/components/input/TextField.rhf.tsx → src/utils/testIdUtils.ts
- `DeleteConfirmationDialogProps` --inherits--> `TestIdProps`  [EXTRACTED]
  src/components/ui/DeleteConfirmationDialog.tsx → src/utils/testIdUtils.ts
- `DeleteConfirmationDialog()` --calls--> `getTestId()`  [EXTRACTED]
  src/components/ui/DeleteConfirmationDialog.tsx → src/utils/testIdUtils.ts

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Tag-triggered release to GitHub Packages** — _github_workflows_release_release_workflow, _github_workflows_release_publish_job, readme_github_packages, _github_workflows_release_tag_driven_versioning [EXTRACTED 1.00]

## Communities (33 total, 11 thin omitted)

### Community 0 - "Core UI Primitives"
Cohesion: 0.10
Nodes (20): Badge(), IBadgeProps, BadgeVariants, ColorSwatch(), IColorSwatchProps, colorSwatchVariants, IMeterProps, Meter() (+12 more)

### Community 1 - "Package Metadata"
Cohesion: 0.04
Nodes (46): description, devDependencies, @biomejs/biome, react, react-dom, react-hook-form, @types/node, @types/react (+38 more)

### Community 2 - "Select Component"
Cohesion: 0.07
Nodes (32): SelectField(), SelectFieldProps, Checkbox, ILogLineProps, JsonObject, LogLine, LogViewerLine, NUMERIC_LEVELS (+24 more)

### Community 3 - "Form System & RHF Fields"
Cohesion: 0.12
Nodes (19): Alert, AlertDescription, AlertTitle, alertVariants, ApiStatusQuery, IApiStatusHandlerProps, ConfirmByTypingDialog(), IConfirmByTypingDialogProps (+11 more)

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
Cohesion: 0.09
Nodes (22): Accordion, AccordionContent, AccordionItem, AccordionTrigger, ISectionHeaderProps, SectionHeader(), NavItem, NavItemProps (+14 more)

### Community 11 - "Button & Calendar Field"
Cohesion: 0.08
Nodes (23): compilerOptions, allowSyntheticDefaultImports, declaration, declarationMap, emitDeclarationOnly, esModuleInterop, isolatedModules, jsx (+15 more)

### Community 12 - "Dropdown Menu"
Cohesion: 0.17
Nodes (11): TextField(), TextFieldProps, EntityPickerLabels, EntityPickerList(), EntityPickerListProps, PickableEntity, Input, InputProps (+3 more)

### Community 13 - "Table Component"
Cohesion: 0.12
Nodes (21): EmptyState(), EmptyStateTone, IEmptyStateProps, EmptyStateRow(), IEmptyStateRowProps, emptyStateBareIconVariants, emptyStateDescriptionVariants, emptyStateIconTileSize (+13 more)

### Community 14 - "Card Component"
Cohesion: 0.16
Nodes (17): Card, CardContent, CardDescription, CardDivProps, CardFooter, CardHeader, CardTitle, DangerZoneCard() (+9 more)

### Community 16 - "biome.json"
Cohesion: 0.17
Nodes (9): FormControl, FormDescription, FormFieldContext, FormFieldContextValue, FormItem, FormItemContext, FormItemContextValue, FormLabel (+1 more)

### Community 17 - "rules"
Cohesion: 0.18
Nodes (10): DropdownMenuCheckboxItem, DropdownMenuContent, DropdownMenuItem, DropdownMenuLabel, DropdownMenuRadioItem, DropdownMenuSeparator, DropdownMenuShortcut(), DropdownMenuSubContent (+2 more)

### Community 18 - "CLAUDE.md"
Cohesion: 0.33
Nodes (6): Build Job, CI Workflow, Publish Job, Release Workflow, Tag-driven Version Alignment, GitHub Packages Registry

### Community 29 - "IconTile.tsx"
Cohesion: 0.24
Nodes (9): IconTile(), IconTileShape, IconTileSize, IconTileTone, IIconTileProps, iconTileVariants, AddTile, IAddTileProps (+1 more)

### Community 30 - "formatter"
Cohesion: 0.52
Nodes (4): INumberedStep, INumberedStepsProps, NumberedSteps(), numberedStepMarkerVariants

### Community 32 - "NumberedSteps.tsx"
Cohesion: 0.06
Nodes (47): Button, CalendarFieldProps, ColorPicker(), ColorPickerCustomProps, DEFAULT_COLORS, SliderField(), SliderFieldProps, Switch() (+39 more)

## Knowledge Gaps
- **235 isolated node(s):** `$schema`, `enabled`, `clientKind`, `useIgnoreFile`, `ignoreUnknown` (+230 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **11 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `cn()` connect `Core UI Primitives` to `NumberedSteps.tsx`, `Select Component`, `Form System & RHF Fields`, `Badge & Sidebar Navigation`, `Dialogs & Color Picker`, `Tabs Component`, `Dropdown Menu`, `Table Component`, `Card Component`, `biome.json`, `rules`, `IconTile.tsx`, `formatter`?**
  _High betweenness centrality (0.243) - this node is a cross-community bridge._
- **Why does `LogViewerActions()` connect `Select Component` to `Core UI Primitives`, `Package Metadata`?**
  _High betweenness centrality (0.163) - this node is a cross-community bridge._
- **Why does `url` connect `Package Metadata` to `Select Component`?**
  _High betweenness centrality (0.160) - this node is a cross-community bridge._
- **What connects `$schema`, `enabled`, `clientKind` to the rest of the system?**
  _236 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Core UI Primitives` be split into smaller, more focused modules?**
  _Cohesion score 0.1021021021021021 - nodes in this community are weakly interconnected._
- **Should `Package Metadata` be split into smaller, more focused modules?**
  _Cohesion score 0.043478260869565216 - nodes in this community are weakly interconnected._
- **Should `Select Component` be split into smaller, more focused modules?**
  _Cohesion score 0.07467532467532467 - nodes in this community are weakly interconnected._