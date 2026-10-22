# Graph Report - design-system  (2026-10-22)

## Corpus Check
- 111 files · ~20,965 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 514 nodes · 1111 edges · 37 communities (26 shown, 11 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS · INFERRED: 1 edges (avg confidence: 0.95)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `c709de1b`
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
- [[_COMMUNITY_correctness|correctness]]
- [[_COMMUNITY_SliderField.rhf.tsx|SliderField.rhf.tsx]]
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
- [[_COMMUNITY_cn|cn]]
- [[_COMMUNITY_styleUtils.ts|styleUtils.ts]]
- [[_COMMUNITY_NumberedSteps.tsx|NumberedSteps.tsx]]
- [[_COMMUNITY_selectContent.tsx|selectContent.tsx]]
- [[_COMMUNITY_accordion.tsx|accordion.tsx]]
- [[_COMMUNITY_repository|repository]]
- [[_COMMUNITY_graphify|graphify]]

## God Nodes (most connected - your core abstractions)
1. `getTestId()` - 90 edges
2. `TestIdProps` - 88 edges
3. `cn()` - 82 edges
4. `compilerOptions` - 20 edges
5. `formatter` - 13 edges
6. `correctness` - 12 edges
7. `Label` - 11 edges
8. `@flightroom/design-system` - 11 edges
9. `formatter` - 10 edges
10. `Button` - 9 edges

## Surprising Connections (you probably didn't know these)
- `SelectField()` --calls--> `getTestId()`  [EXTRACTED]
  src/components/input/SelectField.rhf.tsx → src/utils/testIdUtils.ts
- `ISelectControlProps` --inherits--> `TestIdProps`  [EXTRACTED]
  src/components/ui/select/partials/selectControl/selectControl.tsx → src/utils/testIdUtils.ts
- `TextareaProps` --inherits--> `TestIdProps`  [EXTRACTED]
  src/components/ui/textarea.tsx → src/utils/testIdUtils.ts
- `Build Job` --semantically_similar_to--> `Publish Job`  [INFERRED] [semantically similar]
  .github/workflows/ci.yml → .github/workflows/release.yml
- `Publish Job` --references--> `GitHub Packages Registry`  [EXTRACTED]
  .github/workflows/release.yml → README.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Tag-triggered release to GitHub Packages** — _github_workflows_release_release_workflow, _github_workflows_release_publish_job, readme_github_packages, _github_workflows_release_tag_driven_versioning [EXTRACTED 1.00]

## Communities (37 total, 11 thin omitted)

### Community 0 - "Core UI Primitives"
Cohesion: 0.17
Nodes (10): Badge(), IBadgeProps, BadgeVariants, ColorSwatch(), IColorSwatchProps, colorSwatchVariants, IMeterProps, Meter() (+2 more)

### Community 1 - "Package Metadata"
Cohesion: 0.15
Nodes (12): description, engines, node, files, license, main, module, name (+4 more)

### Community 2 - "Select Component"
Cohesion: 0.10
Nodes (27): CalendarField(), CalendarFieldProps, SelectField(), SelectFieldProps, Spinner(), SpinnerProps, PopoverContent, PopoverTrigger (+19 more)

### Community 3 - "Form System & RHF Fields"
Cohesion: 0.06
Nodes (57): ColorPicker(), ColorPickerCustomProps, DEFAULT_COLORS, SliderField(), SliderFieldProps, Switch(), SwitchCustomProps, TextareaChipsField() (+49 more)

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
Cohesion: 0.15
Nodes (13): Button, spinnerSizeByButtonSize, ButtonVariants, IButtonProps, CopyButton, ICopyButtonProps, CodeBlock(), ICodeBlockProps (+5 more)

### Community 9 - "Dev Dependencies"
Cohesion: 0.07
Nodes (30): noArguments, noExtraBooleanCast, noUselessCatch, noUselessTypeConstraint, noConstantCondition, noConstAssign, noPrecisionLoss, noSelfAssign (+22 more)

### Community 10 - "Tabs Component"
Cohesion: 0.08
Nodes (23): Accordion, AccordionContent, AccordionItem, AccordionTrigger, DeleteConfirmationDialogProps, ISectionHeaderProps, SectionHeader(), NavItem (+15 more)

### Community 11 - "Button & Calendar Field"
Cohesion: 0.08
Nodes (23): compilerOptions, allowSyntheticDefaultImports, declaration, declarationMap, emitDeclarationOnly, esModuleInterop, isolatedModules, jsx (+15 more)

### Community 12 - "Dropdown Menu"
Cohesion: 0.18
Nodes (10): DropdownMenuCheckboxItem, DropdownMenuContent, DropdownMenuItem, DropdownMenuLabel, DropdownMenuRadioItem, DropdownMenuSeparator, DropdownMenuShortcut(), DropdownMenuSubContent (+2 more)

### Community 13 - "Table Component"
Cohesion: 0.12
Nodes (21): EmptyState(), EmptyStateTone, IEmptyStateProps, EmptyStateRow(), IEmptyStateRowProps, emptyStateBareIconVariants, emptyStateDescriptionVariants, emptyStateIconTileSize (+13 more)

### Community 14 - "Card Component"
Cohesion: 0.18
Nodes (15): Card, CardContent, CardDescription, CardDivProps, CardFooter, CardHeader, CardTitle, DangerZoneCard() (+7 more)

### Community 16 - "correctness"
Cohesion: 0.15
Nodes (13): devDependencies, @biomejs/biome, react, react-dom, react-hook-form, @types/node, @types/react, @types/react-dom (+5 more)

### Community 17 - "SliderField.rhf.tsx"
Cohesion: 0.17
Nodes (9): FormControl, FormDescription, FormFieldContext, FormFieldContextValue, FormItem, FormItemContext, FormItemContextValue, FormLabel (+1 more)

### Community 18 - "CLAUDE.md"
Cohesion: 0.33
Nodes (6): Build Job, CI Workflow, Publish Job, Release Workflow, Tag-driven Version Alignment, GitHub Packages Registry

### Community 29 - "IconTile.tsx"
Cohesion: 0.24
Nodes (9): IconTile(), IconTileShape, IconTileSize, IconTileTone, IIconTileProps, iconTileVariants, AddTile, IAddTileProps (+1 more)

### Community 30 - "cn"
Cohesion: 0.33
Nodes (6): scripts, build, dev, format, lint, typecheck

### Community 31 - "styleUtils.ts"
Cohesion: 0.40
Nodes (5): exports, ./package.json, ./theme.css, import, types

### Community 32 - "NumberedSteps.tsx"
Cohesion: 0.52
Nodes (4): INumberedStep, INumberedStepsProps, NumberedSteps(), numberedStepMarkerVariants

### Community 33 - "selectContent.tsx"
Cohesion: 0.50
Nodes (4): peerDependencies, react, react-dom, react-hook-form

### Community 34 - "accordion.tsx"
Cohesion: 0.67
Nodes (3): publishConfig, access, registry

### Community 35 - "repository"
Cohesion: 0.67
Nodes (3): repository, type, url

## Knowledge Gaps
- **233 isolated node(s):** `$schema`, `enabled`, `clientKind`, `useIgnoreFile`, `ignoreUnknown` (+228 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **11 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `TestIdProps` connect `Tabs Component` to `Core UI Primitives`, `NumberedSteps.tsx`, `Select Component`, `Form System & RHF Fields`, `Badge & Sidebar Navigation`, `Dialogs & Color Picker`, `Dropdown Menu`, `Table Component`, `Card Component`, `SliderField.rhf.tsx`, `IconTile.tsx`?**
  _High betweenness centrality (0.089) - this node is a cross-community bridge._
- **Why does `getTestId()` connect `Form System & RHF Fields` to `Core UI Primitives`, `NumberedSteps.tsx`, `Select Component`, `Badge & Sidebar Navigation`, `Dialogs & Color Picker`, `Tabs Component`, `Dropdown Menu`, `Table Component`, `Card Component`, `SliderField.rhf.tsx`, `IconTile.tsx`?**
  _High betweenness centrality (0.078) - this node is a cross-community bridge._
- **Why does `cn()` connect `Select Component` to `Core UI Primitives`, `NumberedSteps.tsx`, `Form System & RHF Fields`, `Badge & Sidebar Navigation`, `Dialogs & Color Picker`, `Tabs Component`, `Dropdown Menu`, `Table Component`, `Card Component`, `SliderField.rhf.tsx`, `IconTile.tsx`?**
  _High betweenness centrality (0.062) - this node is a cross-community bridge._
- **What connects `$schema`, `enabled`, `clientKind` to the rest of the system?**
  _234 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Select Component` be split into smaller, more focused modules?**
  _Cohesion score 0.1014799154334038 - nodes in this community are weakly interconnected._
- **Should `Form System & RHF Fields` be split into smaller, more focused modules?**
  _Cohesion score 0.05574229691876751 - nodes in this community are weakly interconnected._
- **Should `TypeScript Config` be split into smaller, more focused modules?**
  _Cohesion score 0.0524390243902439 - nodes in this community are weakly interconnected._