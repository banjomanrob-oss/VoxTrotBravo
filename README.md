VoxTrotBravo PCVR

VoxTrotBravo is a high-performance, web-based VR voxel engine designed for creative building, sculpting, and architectural prototyping. Built with Three.js and optimized for PCVR (Quest 3/Pro via Link/AirLink), it leverages advanced instancing and a chunk-based architecture to support massive voxel counts at 90Hz/120Hz.

🚀 Quick Start

Open the index.html in a WebXR-compatible browser (Chrome or Edge recommended).

Connect your VR headset to your PC.

Click the Enter VR button at the bottom of the screen.

🎮 Universal Controls

Navigation & World Manipulation

Both Grips (Hold): Grab the air with both hands to move, rotate, and scale the entire world.

Right Grip (Hold): Move the world relative to your right hand.

Left Grip (Hold): Move the world relative to your left hand.

Drawing & Interaction

Right Trigger: Primary Action (Draw, Select, or Interact with Sliders).

Left Trigger: Secondary Action (Erase or Drop/Cancel Selection).

Joysticks: Adjust HSL values of the active color slot (configurable in the Color Menu).

Menus

Right A-Button: Toggle Tools Menu (Right Hand).

Right B-Button: Toggle Global Settings (Right Hand).

Left X-Button: Toggle Tool Options (Left Hand).

Left Y-Button: Toggle Materials & Colors (Left Hand).

🛠 The Toolset

VoxTrotBravo features 12 specialized tools, selectable from the Right Menu (X-Button).

1. Brush (Standard)

The basic building block.

Shapes: Cube or Sphere.

Modes: Solid (fills volume) or Shell (surface only).

Radius: Adjustable from 1 to 10.

2. Extrude (Pull)

Pull existing voxels along an axis.

Modes: Free (auto-snaps to nearest axis), X, Y, or Z.

Adjoining: Toggle to pull all connected voxels of the same color/material simultaneously.

Hollow: Extrude only the outer surface of the volume.

3. Line & Arc Tool

Create straight lines or complex Bezier arcs.

Two-Hand Mode: Stretch a line between your left and right controllers.

Sheet Mode: Extrude a flat surface between two hands.

Arc Control: Adjust the "Bulge" (depth) and "Tilt" via sliders or dynamic wrist pitch.

Gradient Mode: Automatically lerp colors from the start to the end of the stroke.

4. Paint (Recolor)

Change the color or material of existing voxels.

Brush Paint: Standard paint behavior.

Bucket Fill: Flood-fill connected voxels of the same color.

5. Soft Sculpt

A probabilistic brush for organic terrain or cloud-like structures.

Density: Controls the "noise" or thickness of the placement.

6. Box / Volumes

Generate massive rectangular structures instantly.

Wireframe Mode: Create hollow frames with adjustable thickness.

Divisions: Subdivide the box into internal grids or surface segments.

7. Quad Sphere

Creates ellipsoids centered on your draw point.

Solid/Shell: Toggle between full volumes or hollow spheres.

8. Cylinder / Prism

Generates round or polygonal extruded shapes.

Sides: 0 (Perfectly Round) to 32 (Polygon).

Caps: Toggle whether the ends of the cylinder are filled.

9. Triangle (Cone / Pyramid)

Create pointed structures on a specific axis.

Legs: 3 (Tetrahedron) to 12 (High-detail pyramid).

10. Poly / Platonic

Spawn complex geometric solids.

Types: Tetrahedron, Octahedron, Icosahedron, Dodecahedron.

Divisions: Increase the "frequency" of the faces for smoother shapes.

11. Plane (2D Grid)

Lay down flat sheets or outlines.

Thickness: Set the "depth" of the plane (1 to 20 voxels).

Grid: Overlay a secondary grid pattern on the surface.

12. Select & Transform

The most powerful tool for architectural editing.

Selection Modes: Box (area) or Connected (all attached voxels).

Transformations: * Move: Shift selection to a new location.

Copy: Stamp a new copy of the selection.

Free: Bind the selection to your controller for intuitive hand-rotation and scaling.

Draw/Paint: Use your selection as a brush to stamp complex patterns.

Pivot Point: Click "Set Pivot" to choose the rotation/scale center of your selection.

Golden Ratio: A shortcut to scale selections by $\phi$ (1.618).

🎨 Materials & Colors

VoxTrotBravo uses a Dual-Slot Material System (Color A and Color B).

Material Types:

Solid: Standard matte finish.

Glass: Transparent with refraction.

Emission: Self-illuminated (Glow).

Metal: Highly reflective with environment mapping.

Color Modes:

Solid: Uses Color A.

Gradient (H/V): Procedurally blends between Color A and Color B.

Dropper: Sample colors and materials directly from the world by clicking on existing voxels.

⚙️ Advanced Features

Symmetry Systems

Mirrors: Simultaneous mirroring across X, Y, and Z axes.

Polar Symmetry: Radial repetition (1 to 16-fold) for creating mandalas, wheels, or complex circular architecture.

Vertical Lock: Restricts world rotation to the Y-axis to keep your "floor" level.

Performance & Rendering

Standard Mode: High-fidelity instanced meshes with shadows and reflections.

Performance Mode: Switches to a point-cloud renderer, allowing for millions of voxels with lower GPU overhead.

Undo System: Supports up to 10 steps of complex voxel operations.

Export Pipeline

Export Mode: Choose between "Boxes" (individual cubes for voxel aesthetic) or "Mesh" (optimized surface geometry).

OBJ Export: Saves your creation as a standard .obj file.

Note: This uses a streaming writer to prevent browser crashes during massive exports.

⚠️ Requirements

VR Setup: Oculus/Meta Quest 3 or Pro (recommended), Valve Index, or Vive.

Browser: Chrome or Microsoft Edge (Latest versions for WebXR support).

Hardware: A dedicated GPU is required for high voxel counts.
