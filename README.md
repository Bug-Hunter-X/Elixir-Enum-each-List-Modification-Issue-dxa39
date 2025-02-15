# Elixir Enum.each and List Modification

This example demonstrates a common pitfall when attempting to modify a list within an `Enum.each` loop in Elixir.  The code attempts to remove the element `3` from the list, but because `List.delete` creates a *new* list, the original list remains unchanged. 

The solution shows the correct approach using `Enum.filter` to create a new list.