# Tweakpane plugin template
Plugin cva of an input binding for [Tweakpane][tweakpane].




# For plugin users


## Installation


### Browser
```html
<script src="tweakpane.min.js"></script>
<scirpt src="tweakpane-plugin-cva.min.js"></script>
<script>
  const pane = new Tweakpane.Pane();
  pane.registerPlugin(TweakpaneCvaPlugin);
</script>
```


### Package
```js
import {Pane} from 'tweakpane';
import * as CvaPlugin from 'tweakpane-plugin-cva';

const pane = new Pane();
pane.registerPlugin(CvaPlugin);
```


## Usage
```js
const params = {
  prop: 3,
};

// TODO: Update parameters for your plugin
pane.addInput(params, 'prop', {
  view: 'dots',
}).on('change', (ev) => {
  console.log(ev.value);
});
```


[tweakpane]: https://github.com/cocopon/tweakpane/
