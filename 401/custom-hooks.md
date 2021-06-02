# Custom Hooks

## Lifecycle
  - Mounting: Component rendered to DOM
  - Updating: Rerendering that component due to changes
  - Unmounting: when a component is removed from the DOM

## Wrapping with useCallback

This is to ensure the componnet is rendered only when it is needed. UseEffect will trigger the element more often then desired.

## Function vs. Class

Class based components  development requires programmers to track props and elelment up and down the DOM to get data where it needs to go. With functional programming these elements can share data and states more easily and directly with out having to send props and state all the way back to the parent elelement.

## Problem code

UseEffect should only be used on top level, using it in a for loop may lead to infinite looping and rendering. 

## Preview
- async loops still confuse me, how do i know where to put the await?
- is UseReducer as ubiquidous as .reduce?
- Im really excited to get this and bootstrap working together.