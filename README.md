## System Logic: The Rotary Wheel
```mermaid
graph LR
    User([User Interaction]) --> Logic{Index Manager}
    Logic -->|Move Left/Right| Render[Update CSS Classes]
    Render --> Transform[CSS 3D Transform: rotateY / translateZ]
    Render --> VarUpdate[Update --accent-glow Variable]
    VarUpdate --> Visuals[Apply Backdrop Blur & Neon Bleed]
