# WebGPU XPBD Cloth Simulator

This is a WebGPU Cloth Simulator that uses XPBD (extended position based dynamics) with small step sizes.

This relies heavily on the following papers:
- [XPBD: Position-Based Simulation of Compliant Constrained Dynamics - Macklin et. al - NVIDIA](https://matthias-research.github.io/pages/publications/XPBD.pdf)
- [Small Steps in Physics Simulation, Macklin et. al - NVIDIA](https://matthias-research.github.io/pages/publications/smallsteps.pdf)
- [A Survey on Position Based Dynamics, 2017](http://mmacklin.com/2017-EG-CourseNotes.pdf)

As well as code snippets from:
- [Cloth simulation code - Matthias Müller](https://github.com/matthias-research/pages/blob/master/tenMinutePhysics/14-cloth.html)

## Development

The following steps describe how to run this simulation locally.

**Note** - This has only been tested on Windows (specifically WSL2). 

### Accessing the WebGPU API

WebGPU is currently a developmental feature, and thus requires a browser that enables access to it. [Google Canary](https://www.google.com/chrome/canary/) is a good candidate. To enable the correct features in your browser, please do the following:

- Enable the `#enable-unsafe-webgpu` flag in about://flags.

### Running the dev server 

With yarn installed, run the following:

```
yarn
yarn start
```

## Current implementation

- [x] [XPBD Simulation Loop]()
- [x] [Small Steps]()
- [x] [Constraints - Distance]()
- [x] [Constraints - Fast Performant Bending]()
- [x] [Constraints - Isometric Bending]()
- [ ] Constraints - Angular Bending
- [ ] Constraints - Collisions (Self)
- [ ] Constraints - Collisions (External)
- [ ] Damping