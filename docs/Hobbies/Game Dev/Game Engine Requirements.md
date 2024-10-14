As of right now, several popular game engines have fairly large drawbacks in some form or another. Here, I'm making a list of requirements to narrow down my search for a game engine that best suits my needs.

### Requirements


1) Large World Support via double precision floating point
2) Extensible character movement 
3) Inverse Kinematics + Reliable Animation Workflow
4) Decent Networking Solution
5) Terrain Editor
6) Minimalist API
7) Languages: C#, Python, C++
8) Workflow for whiteboxing levels
9) Sane Input scheme

### Godot

Cons:
Stupid UI. No multiscreen support, buttons don't do what you think they should do, etc
Very opinionated composition
No terrain
Broken IK
Basic input scheme
Weird object orientation requiring registering classes via addressing in a gross way
GDScript sucks ass

Pros:
Large world support
Extensible characters, but not great
Okay networking. It at least supports it out of the box
C# support

### UE5

Cons: 
Overly heavy
Intrusive API
Opinionated workflow
Terrible whiteboxing
Complex networking API
Complex animation system
Poor extensibility for CMC

Pros:
Great input scheme
Good terrain editor
Supports IK 
C++
Large Worlds

