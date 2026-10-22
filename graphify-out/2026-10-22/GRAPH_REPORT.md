# Graph Report - design-system  (2026-10-20)

## Corpus Check
- 111 files · ~20,658 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 513 nodes · 1111 edges · 35 communities (24 shown, 11 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS · INFERRED: 2 edges (avg confidence: 0.95)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `764b43b1`
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

## God Nodes (most connected - your core abstractions)
1. `getTestId()` - 90 edges
2. `TestIdProps` - 88 edges
3. `cn()` - 82 edges
4. `compilerOptions` - 20 edges
5. `formatter` - 13 edges
6. `correctness` - 12 edges
7. `Label` - 11 edges
8. `@mfe-orchestrator/design-system` - 11 edges
9. `formatter` - 10 edges
10. `Button` - 9 edges

## Surprising Connections (you probably didn't know these)
- `Build Job` --references--> `@mfe-orchestrator/design-system`  [INFERRED]
  .github/workflows/ci.yml → README.md
- `SelectField()` --calls--> `getTestId()`  [EXTRACTED]
  src/components/input/SelectField.rhf.tsx → src/utils/testIdUtils.ts
- `SliderField()` --calls--> `getTestId()`  [EXTRACTED]
  src/components/input/SliderField.rhf.tsx → src/utils/testIdUtils.ts
- `TextareaField()` --calls--> `getTestId()`  [EXTRACTED]
  src/components/input/TextareaField.rhf.tsx → src/utils/testIdUtils.ts
- `ISelectControlProps` --inherits--> `TestIdProps`  [EXTRACTED]
  src/components/ui/select/partials/selectControl/selectControl.tsx → src/utils/testIdUtils.ts

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Tag-triggered release to GitHub Packages** — _github_workflows_release_release_workflow, _github_workflows_release_publish_job, readme_github_packages, _github_workflows_release_tag_driven_versioning [EXTRACTED 1.00]

## Communities (35 total, 11 thin omitted)

### Community 0 - "Core UI Primitives"
Cohesion: 0.17
Nodes (10): Badge(), IBadgeProps, BadgeVariants, ColorSwatch(), IColorSwatchProps, colorSwatchVariants, IMeterProps, Meter() (+2 more)

### Community 1 - "Package Metadata"
Cohesion: 0.04
Nodes (46): description, devDependencies, @biomejs/biome, react, react-dom, react-hook-form, @types/node, @types/react (+38 more)

### Community 2 - "Select Component"
Cohesion: 0.15
Nodes (15): SelectField(), SelectFieldProps, SelectContent, ISelectControlProps, SelectControl(), SelectControlContext, SelectControlContextValue, SelectItem (+7 more)

### Community 3 - "Form System & RHF Fields"
Cohesion: 0.06
Nodes (43): Button, ColorPicker(), ColorPickerCustomProps, Switch(), SwitchCustomProps, TextareaChipsField(), TextareaChipsFieldProps, TextField() (+35 more)

### Community 4 - "TypeScript Config"
Cohesion: 0.08
Nodes (23): compilerOptions, allowSyntheticDefaultImports, declaration, declarationMap, emitDeclarationOnly, esModuleInterop, isolatedModules, jsx (+15 more)

### Community 5 - "Runtime Dependencies"
Cohesion: 0.08
Nodes (24): dependencies, class-variance-authority, clsx, date-fns, lucide-react, @radix-ui/react-accordion, @radix-ui/react-avatar, @radix-ui/react-checkbox (+16 more)

### Community 6 - "Docs & CI/CD Pipeline"
Cohesion: 0.12
Nodes (16): Build Job, CI Workflow, Publish Job, Release Workflow, Tag-driven Version Alignment, Accessibilità, Contenuto, GitHub Packages Registry (+8 more)

### Community 7 - "Badge & Sidebar Navigation"
Cohesion: 0.11
Nodes (24): TextareaField(), TextFieldProps, DeleteConfirmationDialogProps, DescriptionItem(), IDescriptionItemProps, DescriptionList(), DescriptionListContext, DescriptionListOrientation (+16 more)

### Community 8 - "Dialogs & Color Picker"
Cohesion: 0.16
Nodes (12): spinnerSizeByButtonSize, ButtonVariants, IButtonProps, CopyButton, ICopyButtonProps, CodeBlock(), ICodeBlockProps, codeBlockVariants (+4 more)

### Community 9 - "Dev Dependencies"
Cohesion: 0.15
Nodes (11): DEFAULT_COLORS, Avatar, AvatarFallback, AvatarImage, Checkbox, RadioGroup, RadioGroupItem, TabsContent (+3 more)

### Community 10 - "Tabs Component"
Cohesion: 0.23
Nodes (7): TabsList, tabsListVariants, TabsTrigger, tabsTriggerVariants, Tabs, TabsContext, TabsProps

### Community 11 - "Button & Calendar Field"
Cohesion: 0.05
Nodes (40): source, assist, actions, enabled, css, parser, files, ignoreUnknown (+32 more)

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
Cohesion: 0.07
Nodes (30): noArguments, noExtraBooleanCast, noUselessCatch, noUselessTypeConstraint, noConstantCondition, noConstAssign, noPrecisionLoss, noSelfAssign (+22 more)

### Community 17 - "SliderField.rhf.tsx"
Cohesion: 0.21
Nodes (9): SliderField(), SliderFieldProps, Slider, SliderProps, ToggleGroup, ToggleGroupContext, ToggleGroupItem, Toggle (+1 more)

### Community 29 - "IconTile.tsx"
Cohesion: 0.24
Nodes (9): IconTile(), IconTileShape, IconTileSize, IconTileTone, IIconTileProps, iconTileVariants, AddTile, IAddTileProps (+1 more)

### Community 30 - "cn"
Cohesion: 0.22
Nodes (9): CalendarField(), CalendarFieldProps, Spinner(), SpinnerProps, PopoverContent, PopoverTrigger, ISectionHeaderProps, SectionHeader() (+1 more)

### Community 31 - "styleUtils.ts"
Cohesion: 0.39
Nodes (3): SelectLabel, selectLabelVariants, navItemVariants

### Community 32 - "NumberedSteps.tsx"
Cohesion: 0.52
Nodes (4): INumberedStep, INumberedStepsProps, NumberedSteps(), numberedStepMarkerVariants

### Community 33 - "selectContent.tsx"
Cohesion: 0.53
Nodes (3): selectContentVariants, SelectScrollDownButton, SelectScrollUpButton

### Community 34 - "accordion.tsx"
Cohesion: 0.40
Nodes (4): Accordion, AccordionContent, AccordionItem, AccordionTrigger

## Knowledge Gaps
- **232 isolated node(s):** `$schema`, `enabled`, `clientKind`, `useIgnoreFile`, `ignoreUnknown` (+227 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **11 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `TestIdProps` connect `Badge & Sidebar Navigation` to `Core UI Primitives`, `NumberedSteps.tsx`, `Select Component`, `Form System & RHF Fields`, `accordion.tsx`, `selectContent.tsx`, `Dialogs & Color Picker`, `Dev Dependencies`, `Tabs Component`, `Dropdown Menu`, `Table Component`, `Card Component`, `SliderField.rhf.tsx`, `IconTile.tsx`, `cn`, `styleUtils.ts`?**
  _High betweenness centrality (0.089) - this node is a cross-community bridge._
- **Why does `getTestId()` connect `Form System & RHF Fields` to `Core UI Primitives`, `NumberedSteps.tsx`, `Select Component`, `accordion.tsx`, `selectContent.tsx`, `Badge & Sidebar Navigation`, `Dialogs & Color Picker`, `Dev Dependencies`, `Tabs Component`, `Dropdown Menu`, `Table Component`, `Card Component`, `SliderField.rhf.tsx`, `IconTile.tsx`, `cn`, `styleUtils.ts`?**
  _High betweenness centrality (0.078) - this node is a cross-community bridge._
- **Why does `cn()` connect `cn` to `Core UI Primitives`, `NumberedSteps.tsx`, `accordion.tsx`, `Form System & RHF Fields`, `selectContent.tsx`, `Select Component`, `Badge & Sidebar Navigation`, `Dialogs & Color Picker`, `Dev Dependencies`, `Tabs Component`, `Dropdown Menu`, `Table Component`, `Card Component`, `SliderField.rhf.tsx`, `IconTile.tsx`, `styleUtils.ts`?**
  _High betweenness centrality (0.062) - this node is a cross-community bridge._
- **What connects `$schema`, `enabled`, `clientKind` to the rest of the system?**
  _233 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Package Metadata` be split into smaller, more focused modules?**
  _Cohesion score 0.043478260869565216 - nodes in this community are weakly interconnected._
- **Should `Select Component` be split into smaller, more focused modules?**
  _Cohesion score 0.14624505928853754 - nodes in this community are weakly interconnected._
- **Should `Form System & RHF Fields` be split into smaller, more focused modules?**
  _Cohesion score 0.06284153005464481 - nodes in this community are weakly interconnected._