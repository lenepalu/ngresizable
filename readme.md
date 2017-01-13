# Angular Resizable

Simple, tree-shakable, AoT, Universal and WebWorkers friendly resizable component for Angular (2 and beyond).

# API

## Outputs

  - `resizeStart: EventEmitter<IResizeEvent>` - Resize start event.
  - `resizing: EventEmitter<IResizeEvent>` - Resizing event.
  - `resizeEnd: EventEmitter<IResizeEvent>` - Resize end event.

## Inputs

  - `width` - Width of the element number.
  - `height: number` - Height of the element.
  - `x: number` - x coordinate of the element.
  - `y: number` - y coordinate of the element.
  - `maxWidth: number` - Maximum width. Default `Infinity`.
  - `minWidth: number` - Minimum width. Default `0`.
  - `maxHeight: number` - Maximum height. Default `Infinity`.
  - `minHeight: number` - Minimum height. Default `0`.
  - `disableResize: boolean = false` - Disable the resize.
  - `directions: string[]` - An array which contains the resize directions. Default `['bottom', 'right']`.
  - `grid: ISize` - Resize in a grid. Default `{ width: 1, height: 1 }`.
  - `bound: IRectangle` - Bound the resize.
  - `ratio: number` - Resize ratio.

# Integration

Should work out of the box with webpack, respectively angular-cli.

## Angular Seed

```ts
// tools/config/project.ts

...
// Add packages (e.g. ngresizable)
let additionalPackages: ExtendPackages[] = [{
  name: 'ngresizable',
  path: 'node_modules/ngresizable/index.js'
}];

this.addPackagesBundles(additionalPackages);
...
```

# License

MIT
