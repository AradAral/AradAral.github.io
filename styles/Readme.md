# The Architecture of This Sass Project:

Inspired by Hugo Giraudel's 7-1 architecture and Brad Frost's Atomic Design.

All Sass partials are categorized into one of the following groups/folders:
## 1. Abstracts
Sass variables, mixins, functions, etc.
The files in this folder won't output any CSS if transpiled on their own. 
- Config
- Base

## 2. Base
Global and basic CSS
- Global

## 3. Atoms
Micro modules that are completely standalone. They are pure building blocks, they are not composed of any other blocks.
Alternative names:
- Components
- Micros

## 4. Molecules
Macro modules that are composed of atoms/micro modules. Self-contained, but not including layout.
- Modules
- Macros

## 5. Organisms
These are blocks that make up the global wireframe of the project. Most of them are used only once or twice in each web page.
Control layout.
- Layout
- Skeleton
- Scheme

Optional Layers:
## Libraries
Where third-party code is located
Alternative names:
- Vendors
- Plugins
- Addons
If you want to override some of these third-party code, don't modify their files directly, rather, add another folder, called "extensions" inside the vendors fold

app.scss OR main.scss OR all.scss

## Utilities
Alternative names:
- 