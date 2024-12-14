# Unexpected Behavior of map() with Mutable Lists in Kotlin

This example demonstrates a common point of confusion for Kotlin developers new to the language.  The `map()` function, while powerful, does *not* modify the original collection.  Instead, it returns a *new* collection containing the transformed elements.  This is true even for mutable lists.

The provided code shows the `map()` function being used correctly, but highlights the often-overlooked fact that the original `mutableList` remains unchanged.

The `bugSolution.kt` file provides a solution for modifying the original list using `mapIndexedTo` which is shown in the solution section.