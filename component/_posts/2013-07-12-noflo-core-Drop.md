---
  title: "Drop"
  library: "noflo-core"
  layout: "component"

---

```coffeescript
noflo = require 'noflo'

class Drop extends noflo.Component
  description: 'This component drops every packet it receives with no
  action'

  constructor: ->
    @inPorts =
      in: new noflo.Port

    @outPorts = {}

exports.getComponent = -> new Drop

```