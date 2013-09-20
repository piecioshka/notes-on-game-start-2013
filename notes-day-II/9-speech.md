3D for 2D. Anatomy and vivisection of a modern game engine - Ibon Tolosana
==========================================================================

Ibon, CTO @lude @hyperandroid

Antialias 3D context
```
ctx = canvas.getContext('webgl', {
 antialias: boolean
 alpha: boolean 
});
```

14000 spites
1001 svg lion

### Buffer sub data
- 2d in 3d is worst scenarion
- bufferdata is faster than subdata on mobile
- hide buffers perform worse thane smaller buffers 8k-16k traingles

### Animation loop-batch
For each actor/display object
- calculate local matrix 
- calculate gloval matrix 
- set sprite screen bounds (transform 4 points)
- if texture changes or program needs change, flush program -> uploads
buffer to GPU
- store client side calculate color and certices
- repeat forever

### Timing function
- setinterval vs requestanimationframe
- honor raf performance timing
- measure raf and draw time

### Loops
suprises under the good?


FF is at least 3x faster than chrome traversing arrays
Chrome is sensetive to the loop syntax


### JIT and JS
- create properties in constructor function
- keep the number low (30+)
- let the ic do the magic


### What will ruin JIT
- dunamic object properties 
- for-in big code function
- be memory friendly dont allocate in loops
- avoid testing webgl instructions


### What to do when all this has failed
- use smaller context object and scale via css!!!


