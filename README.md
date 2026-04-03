# -Polyline-Editor

# Polyline Editor with 3d view (HCI LAB MOCK MID)
This project was developed as part of the **Human-Computer Interaction (HCI) Mid Lab**.  
During the design process, concepts from **Chapter 5 of the HCI textbook** were studied and applied to guide the interaction design and usability considerations of the system.  


### Phase 3: Design Phase

**Name:** Muhammad Ibrahim  
**Seat No:** B23110006103
## Deployment Link:
https://hcimidlab154.vercel.app/

# Team Members

| Name | Seat No | Phase | Repo Link |
|-----|-----|-----|-----|
| Shaheer Ahmed | B23110006154 | Implementation and Deployment |https://github.com/shaheerahmedcoder/HCI-Polyline-Editor-3d-|
| Muhammad Ibrahim | B23110006103 | Design Phase | https://github.com/muhammadibrahim146/-Polyline-Editor |
| M Bilal Atif Usmani | B23110006057 |Analysis Phase |https://github.com/m-bilal-atif227584/HCI-Lab-PolylineEditor |
| Muhammad Mujtaba | B23110006107 | Requirement Phase |https://github.com/Mujtaba214/HCI-3D-Polyline-Editor-Lab/|


##My contribution
Contribution: Implemented HCI design principles (Chapter 5) in Polyline Editor, focusing on usability, UI flow, and user interaction.

# . System Functionality
## Keyboard Controls

| Key | Action | Description |
|-----|--------|-------------|
| B / N | Begin | Start creating a new polyline |
| D | Delete | Remove the closest vertex |
| M | Move | Pick a vertex and place it at a new location |
| I | Insert | Insert a new point on the nearest segment |
| Z | Undo | Undo the last action (up to 30 steps) |
| R | Refresh | Redraw all polylines on the canvas |
| ESC | End | End current polyline drawing |
| Q | Quit | Clear the canvas and end the session |

# . Additional Functions Added Beyond Basic Requirements

| Function | Implementation |
|--------|--------|
| Undo (Z) | A history stack stores deep-cloned snapshots of `polys[]`. Pressing Z restores the previous state. |
| Export PNG | Canvas content is copied to a temporary canvas and downloaded as a PNG file. |
| Save / Load JSON | Serializes the polyline array into a `.json` file and restores it when loaded. |
| View in 3D | Converts 2D coordinates into a 3D scene rendered using Three.js. |
| Color & Stroke Width | Users can select polyline color and thickness in real time. |


# . Interactive Process

The development followed the **HCI Interaction Design Lifecycle**:

**Requirements → Analysis → Design → Implementation**

---

### Requirements
Requirements gathering was completed in **Phase 1** by **Mujtaba**.

---

### Analysis
During the analysis phase, **Chapter 5 of the HCI textbook** was studied and considered while planning the interaction design.  
The concepts from this chapter helped in understanding **user tasks, interaction flow, and usability considerations** for the polyline editor.

---

### Design
This phase was completed by **Ibrahim**.During the design phase, **Chapter 5 of the HCI textbook** was studied and considered while planning 
Several **HCI principles** were applied in the design, including:

- Direct manipulation
- Immediate visual feedback
- Consistent keyboard shortcuts
- Error prevention

---

### Implementation & Deployment
This phase was completed by **Shaheer Ahmed**.

The final system integrates all the required interaction features and also includes several additional improvements. The implementation focused on:

- Proper use of **data structures** for managing polylines and vertices
- Implementing the **segment insertion mechanism** inside a polyline
- Supporting **keyboard shortcut–based interaction** for efficient editing
- Implementing **undo functionality using a history stack**
- Adding a **3D viewing experience using Three.js** for visualizing polylines in a layered 3D scene

 
 ## Design Process for the Interactive Polyline Editor
 
We followed a user-centered iterative design approach:
1. Requirements Analysis: Identified four core interaction modes (Draw, Move, Delete, Insert) from the course specification, each requiring distinct visual feedback and cursor behavior.
2. Metaphor Selection: Adopted an MS Paint-inspired ribbon toolbar metaphor — familiar to users, reducing learning curve (HCI principle: leverage existing mental models).
3. Feedback Design: Every action produces immediate visual feedback — color-coded mode buttons, vertex glow on hover (red=delete, yellow=move, teal=insert), ghost preview lines, and toast notifications. This satisfies Nielsen's heuristic of visibility of system status.
4. Error Prevention: Auto-removal of polylines with < 2 points, max 100 polyline limit with user notification, and confirmation dialog on Quit.
5. Shortcuts & Efficiency: Single-key shortcuts (B/M/D/I/Z/R/ESC/Q) for expert users alongside clickable buttons for novices — supporting both *recognition and recall*.
6. Iterative Refinement: Moved from dark theme → light MS Paint theme based on feedback, adjusting layout, color tokens, and typography for professional appearance

 ## Challenges Faced
 
During the design process, several challenges were encountered:
Translating theoretical HCI principles into a practical interface design 
Ensuring simplicity while still supporting all required functionalities 
Maintaining consistency across different user interactions (mouse + keyboard) 
Designing an interface that provides real-time feedback without complexity 
Understanding how to apply iteration in a small-scale academic project


## Confusion Faced

During the implementation of the design phase, some confusion was experienced:
Differentiating between analysis and design phases, as both involve thinking about user tasks
Deciding the level of detail required for UI sketches vs actual implementation
Understanding how deeply iteration should be applied in a prototype-level project
However, these confusions were resolved by revisiting Chapter 5 concepts, particularly the distinction between problem understanding (analysis) and solution creation (design).









