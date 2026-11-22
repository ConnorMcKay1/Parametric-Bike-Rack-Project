<h3 align="center">
  Documentation Under Construction . . .
</h3>

<p align="center">
  documentation is under construction, continue to navigate docs & models to view renders, files, and design notes.
</p>

<p align="center">
  <img src="docs/images/renders/materialsTest-assemblyGIF-quality.gif" width="600">
</p>



Parametric-Bike-Rack-Project/
│
├── README.md
│
├── docs/                             # Documentation & engineering record
│   │
│   ├── design notes/                 # Dimensions & design decisions
│   │   ├── Center_Bar_Dimensions.dxf
│   │   ├── Driver-Passenger_Bar_Dimensions.dxf
│   │   ├── TBolt_Dimensions.dxf
│   │   └── roof rack.txt
│   │
│   ├── images/                       # Visual documentation
│   │   ├── dimensions/               # CAD dimension screenshots
│   │   ├── renders/                  # CAD renders & FEA visuals
│   │   └── sketches/                 # Initial concepts & hand sketches
│   │
│   ├── journal/                      # Development history
│   │   ├── journal images/
│   │   ├── 2026-06-28-material-properties-test.md
│   │   ├── 2026-11-17-update.md
│   │   └── 2026-11-21-scripting-workflow.md
│   │
│   ├── research/                     # Technical research
│   │   └── CAD-kernels.md
│   │
│   └── simulations/                  # Engineering simulation
│       ├── FEM/                      # Finite Element Method
│       │   └── structural-simulation.md
│       │
│       └── FVM/                      # Finite Volume Method
│           └── aerodynamic-simulation.md
│
└── models/                           # CAD & computational models
    │
    ├── Roof-Rack_Bike-Rack-V3.FCStd  # Primary CAD assembly
    │
    ├── bike rack u-bolts/            # Custom mounting components
    │   ├── *.FCStd
    │   ├── *.STEP
    │   └── *.FCBak
    │
    ├── *.FCStd                        # FreeCAD models
    ├── *.STEP                         # CAD interchange
    ├── *.DXF                          # Dimension drawings
    └── *.PMX                          # PrePoMax simulation models
