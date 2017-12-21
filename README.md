# Phaser CE Type-updated

This fork makes it easier to use Phaser CE for Typescript development.

## Install

```
npm install --save-dev phaser-ce-type-updated
```

## Usage

```json
// tsconfig.json
{
  ...
  "include": [
    "./node_modules/phaser-ce-type-updated/typescript/phaser.d.ts",
    ...
  ]
}
```

```typescript
// index.ts
import p2 = require('phaser-ce-type-updated/build/custom/p2');
import PIXI = require('phaser-ce-type-updated/build/custom/pixi');
import Phaser = require('phaser-ce-type-updated/build/custom/phaser-split');

(window as any).p2 = p2;
(window as any).PIXI = PIXI;
(window as any).Phaser = Phaser;
```
