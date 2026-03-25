# Web Glass Effect

`web-glass-effect` is a pnpm workspace containing:

- `@creatorem/web-glass-effect`: publishable React package with liquid-glass primitives and controls
- `@creatorem/next-demo`: Next.js app with an iTunes-style mock player and stress panel

## Package

Published package name: `@creatorem/web-glass-effect`

Core exports:

- `LiquidGlass`
- `useLiquidSurface`
- `LiquidFilter`
- `LiquidSlider`
- `LiquidSwitch`
- Surface helpers: `CONVEX`, `CONCAVE`, `LIP`, `WAVE`, `STEPPED`, `ELASTIC`, `BUBBLE`, `CONVEX_CIRCLE`

## Browser compatibility

The SVG `backdrop-filter: url(#filter)` pipeline is Chromium-first. On unsupported engines (for example Safari/Firefox), components degrade to a blur fallback style.

## Install

```bash
pnpm install
```

## Run demo app

```bash
pnpm dev:demo
```

Then open [http://localhost:4100](http://localhost:4100).

## Run Storybook

```bash
pnpm storybook
```

## Run tests

```bash
pnpm test
```

## Verify everything

```bash
pnpm verify
```

## Build

```bash
pnpm build
```

## Publish package

```bash
pnpm --filter @creatorem/web-glass-effect build
pnpm --filter @creatorem/web-glass-effect test
pnpm --filter @creatorem/web-glass-effect publish --access public
```

## Migration note and credits

The implementation is extracted and adapted from the liquid-glass motion components in the Creatorem kit (`liquid-lib`, `filter`, `glass`, `slider`, `switch`) and their docs/examples.

Original inspiration: Chris from kube.io on liquid glass CSS/SVG techniques.
