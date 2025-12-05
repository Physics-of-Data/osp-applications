# OpenSourcePhysics Applications

Interactive physics simulations powered by [OpenSourcePhysics](https://www.compadre.org/osp/) and [CheerpJ](https://cheerpj.com/).

## Live Demo

**Visit**: https://physics-of-data.github.io/osp-applications/

## Applications

### 1. SHO with EJS Controls
- Simple Harmonic Oscillator with modern EJS interface
- Multiple ODE solvers (Euler, Verlet, RK4)
- Real-time visualization and error analysis

### 2. Fixed-Step ODE Solver
- Advanced SHO focusing on fixed-step numerical methods
- 9 different ODE solvers for comparison
- Semi-log error plots with relative/absolute options

### 3. Fixed-Step with Error Logging
- Complete error analysis suite
- Comprehensive data logging table
- Multiple plot windows with configurable intervals

## Technology Stack

- **Framework**: OpenSourcePhysics (OSP)
- **GUI**: EJS (Easy Java Simulations) GroupControl
- **Runtime**: CheerpJ 4.1 (Java 11 support)
- **Deployment**: GitHub Pages

## Repository Structure

```
osp-applications/
├── index.html              # Landing page
├── lib/
│   └── osp.jar            # Shared OSP library (2.3 MB)
└── apps/
    ├── sho-ejs/           # Simple HO with EJS
    ├── fixed-step/        # Fixed-step solver comparison
    └── fixed-step-error/  # With error logging
```

## Key Discovery

EJS applications require **explicit osp.jar in classpath** for CheerpJ:

```javascript
await cheerpjRunMain(
  "your.MainClass",
  "/app/osp-applications/apps/myapp/app.jar:/app/osp-applications/lib/osp.jar"
);
```

See [EJS-CHEERPJ.md](https://github.com/Physics-of-Data/FixedStepErrorLogEjsApp/blob/main/EJS-CHEERPJ.md) for full documentation.

## Credits

- **Physics of Data**: Application development
- **OpenSourcePhysics**: Framework and libraries
- **CheerpJ**: WebAssembly Java runtime

## License

Applications are educational tools for computational physics.
