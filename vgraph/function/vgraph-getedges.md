# getEdges([Labels])
Get Edges optionally filtered by labels.

## Parameters

* [Labels](../definition/element-label.md) - An optional Array of Labels.

## Actions

1. If [Labels](../definition/element-label.md) is set and any [Label](../definition/element-label.md) in [Labels](../definition/element-label.md) is invalid, [Error](../definition/error.md).
1. For each [Edge](../definition/edge.md) in the graph:
    1. If [Status](../definition/element-status.md) is greater than or equal to `4` (Deleted), continue.
    1. If [Labels](../definition/element-label.md) is set and not empty and [Edge's](../definition/edge.md) [Label](../definition/element-label.md) is NOT in [Labels](../definition/element-label.md), continue.
    1. Else return it.


## Returns

An Array or Iterable  of [Edges](../definition/edge.md).