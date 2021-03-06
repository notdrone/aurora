### Tooltip

Tooltip Component

### Props

```table
span: 6
rows:
  - Prop: children
    Type: node
    Default:
    Notes: Render as the Tooltip's children
  - Prop: isVisible
    Type: boolean
    Default: 'false'
    Notes: Show/hide tooltip
  - Prop: variant
    Type: one of 'dark', 'light'
    Default: 'light'
    Notes: Changes tooltip color scheme
  - Prop: direction
    Type: one of 'left', 'right', 'top', 'bottom'
    Default: 'auto'
    Notes: Changes tooltip direction from the item that triggers it. Auto shows the tooltip on top/bottom and makes sure it is always visibel in the view port and in the restriction container that is being passed as second param to getDimensionsFromEvent
  - Prop: position
    Type: Object
    Default: all props are 0
    Notes: This prop is generated from Tooltip.getDimensionsFromEvent(e, parent) static function. The function should receive the event that triggers the Tooltip (usually hover). Secondary parameter that restricts tooltip to be visible in a certain container. Work only if direction is auto
```

```react
---
<div style={{ display: 'flex', justifyContent: 'space-between' }}>
  <TooltipDemo
    direction="bottom"
    text="Hover for Bottom Tooltip"
  />
  <TooltipDemo
    direction="top"
    text="Hover for Top Tooltip"
  />
  <TooltipDemo
    direction="right"
    text="Hover for Right Tooltip"
  />
  <TooltipDemo
    direction="left"
    text="Hover for Left Tooltip"
  />
</div>
```

```react
---
<div>
  <TooltipRestrictedDemo />
</div>
```

### Seat Tooltip

Seat Tooltip Component

### Props

```table
span: 6
rows:
  - Prop: children
    Type: node
    Default:
    Notes: Render as the Seat Tooltip's children
  - Prop: isVisible
    Type: boolean
    Default: 'false'
    Notes: Show/hide tooltip
  - Prop: variant
    Type: one of 'dark', 'light'
    Default: 'light'
    Notes: Changes tooltip color scheme
  - Prop: size
    Type: one of 'small', 'large'
    Default: 'large'
  - Prop: direction
    Type: one of 'left', 'right', 'top', 'bottom'
    Default: 'auto'
    Notes: Changes tooltip direction from the item that triggers it. Auto shows the tooltip on top/bottom and makes sure it is always visibel in the view port and in the restriction container that is being passed as second param to getDimensionsFromEvent
  - Prop: section
    Type: string or number
    Default: n/a
    Notes: Required field. Shows the section in seat data
  - Prop: row
    Type: string or number
    Default: n/a
    Notes: Required field. Shows the row in seat data
  - Prop: seat
    Type: string or number
    Default: n/a
    Notes: Required field. Shows the seat in seat data
  - Prop: position
    Type: Object
    Default: all props are 0
    Notes: This prop is generated from SeatTooltip.getDimensionsFromEvent(e, parent) static function. The function should recieve the event that triggers the Tooltip (usually hover). Secondary parameter that restricts seat tooltip to be visible in a certain container. Work only if direction is auto
```

```react
---
<div>
  <div style={{ display: 'flex', justifyContent: 'space-between' }}>
    <SeatTooltipDemo
      direction="bottom"
      text="Hover for Bottom Tooltip"
    />
    <SeatTooltipDemo
      direction="top"
      text="Hover for Top Tooltip"
    />
    <SeatTooltipDemo
      direction="right"
      text="Hover for Right Tooltip"
    />
    <SeatTooltipDemo
      direction="left"
      text="Hover for Left Tooltip"
    />
  </div>
  <div style={{ display: 'flex', justifyContent: 'space-between', marginTop: '20px' }}>
    <SeatTooltipDemo
      size="small"
      variant="dark"
      direction="bottom"
      text="Hover for Bottom Tooltip"
    />
    <SeatTooltipDemo
      size="small"
      variant="dark"
      direction="top"
      text="Hover for Top Tooltip"
    />
    <SeatTooltipDemo
      size="small"
      variant="dark"
      direction="right"
      text="Hover for Right Tooltip"
    />
    <SeatTooltipDemo
      size="small"
      variant="dark"
      direction="left"
      text="Hover for Left Tooltip"
    />
  </div>
</div>
```
