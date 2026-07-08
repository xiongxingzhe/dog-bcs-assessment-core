# Dog BCS Assessment Core

Minimal helpers for mapping dog Body Condition Score (1-9) to clinical bands.

Built by [pawsandpounds.com](https://pawsandpounds.com).

## Installation

```bash
npm install dog-bcs-assessment-core
```

## Quick Start

```ts
import { dogBcsBand } from "dog-bcs-assessment-core"

dogBcsBand(2) // "underweight"
dogBcsBand(5) // "ideal"
dogBcsBand(7) // "overweight"
dogBcsBand(8) // "obese"
```

## API

### `dogBcsBand(score: number): "underweight" | "ideal" | "overweight" | "obese"`

Rules:
- 1-3 => `underweight`
- 4-5 => `ideal`
- 6-7 => `overweight`
- 8-9 => `obese`

Throws if score is outside `1..9`.

## License

MIT