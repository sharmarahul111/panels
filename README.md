# Panels
Control panel and info panels for my javascript canvas projects inspired by dat.GUI
> With added features to help build game menus, and info boxes quickly

## The Plan
### UI
- a menu with basic style
  - style for the list items
    - text fields
    - sliders
    - toggle
    - color picker
    - select option
    - button
  - folder structure
    - collapse feature
- collapse feature
- transparency
- draggable menu
### UX
- class
- default constructor arguments/setup
- add() to add new component
- remember settings on refresh
- bind events to value change of variable
### Data Structure
- text (string)
- option (array)
- toggle (boolean)
- range (number 0 to 100 by default OR object{min,max,default})
- color (panels.color("color value")),
- button (function)

Initialization example (prototype)
```javascript
let settings = {
  name:"textfield input",
  type: ["opt1", "opt2"],
  on: true,
  speed:20,
  velocity: panels.range(defaultValue, max, min),
  color: panels.color("#00ffd1"),
  doit: function(){},

}
let gui = new Panels(settings)
gui.add() // haven't thought of it yet
```
