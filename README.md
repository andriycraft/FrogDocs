<div class="betterheader" role="banner">
      <h1 class="project-name">GreenFrog</h1>
</div>


## API docs

### Plugin structure

package.json:

```json
{
    "name": "exampleplugin",
    "main": "exampleplugin.js",
    "version": "1.0.0",
    "displayName": "Example plugin",
    "author": "Me",
    "description": "Example plugin to test GreenFrog API"
}
```

code:

```javascript
module.exports = {
  name: "ExamplePlugin",
  version: "1.0", 

  onLoad() {
    Logger.log(`${this.name} > Hello world!`);
  },

  onShutdown() {
    Logger.log(`${this.name} > Good bye!`);
  },
};
```

### Examples

1. Main example plugin > <a href="./data/ExamplePlugin/">Click to open</a> 
2. Send a simple "Hello, world" message on join > <a href="./data/SimpleOnJoin/">Click to open</a>
