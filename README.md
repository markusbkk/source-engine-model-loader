# source-engine-model-loader

three.js loader for parsing source engine models

# Use

```js
import { SourceModelLoader } from 'source-engine-model-loader';

new SourceModelLoader()
  .load( './folder/model', group => {

    scene.add( group );

  } );
```

# API

## SourceModelLoader

### constructor

```js
constructor( manager : LoadingManager )
```

### load

```js
load( url : string, onComplete : Function ) : void
```

Loads the set of Source Engine model files at the given path. It is expected that a model with the extensions `.mdl`, `.vvd`, and `.vtx` exist.

# Unimplemented Features
- Mouths
- Flex controllers / Morph targets
- Levels of detail
- Inverse kinematic chains
- Animation sequences
