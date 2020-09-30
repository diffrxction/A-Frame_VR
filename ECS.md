# Entity-Component-System

## What is the ECS architecture? And how does A-Frame use it?

Module 3 current in maintenance mode.

A-Frame is a three.js framework with an entity-component-system (ECS) architecture. ECS architecture is a common and desirable pattern in game development where every object in the game is an entity (e.g. characters, bullets, vehicles, etc.). And every entity consists of one or more components that contain data or state. Therefore, the behavior of an entity can be changed at runtime by systems that add, remove, or mutate components.

ECS Example

![entity-component-system](https://user-images.githubusercontent.com/65293175/94682054-044fde00-0342-11eb-83bf-362535782464.png)

A basic definition of ECS involves:

  - Entities: Entities are the base of all objects in the scene. They are container objects into which components can be attached. Without components, entities neither do nor render anything, similar to empty `<div>`s.

  - Components: Reusable modules or data containers that can be attached to entities to provide appearance, behavior, and/or functionality. Components are like plug-and-play for objects. All logic is implemented through components, and we define different types of objects by mixing, matching, and configuring components. Like alchemy!

  - Systems provide global scope, management, and services for classes of components. Systems are often optional, but we can use them to separate logic and data; systems handle the logic, components act as data containers.

## Examples

   Box = Position + Geometry + Material

   Sign = Position + Geometry + Material + Text

   Light Bulb = Position + Geometry + Material + Light + Shadow

   Ball = Position + Geometry + Material + Velocity + Physics

   Player = Position + Camera + Input + Avatar + Identity

### ECS in A-Frame

  - Entities are represented by the <a-entity> element and prototype.

  - Components are represented by HTML attributes on <a-entity>‘s. Underneath, components are objects containing a schema, lifecycle handlers, and methods. Components are registered via the AFRAME.registerComponent (name, definition) API.

  - Systems are represented by <a-scene>‘s HTML attributes. System are similar to components in definition. Systems are registered via the AFRAME.registerSystem (name, definition) API.
  
![ecs](https://user-images.githubusercontent.com/65293175/94682118-1b8ecb80-0342-11eb-8b64-a10711886442.gif)
