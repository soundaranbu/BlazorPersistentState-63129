
The `Counter` page component has a `PersistentState` attribute for the currentCount property
- The count persists and restores successfully on page load/refresh
- But it doesn't restore on navigating between pages

The Home page uses another `CounterWithKey` componet with two variations
- One property with `AllowUpdates` set to `true`
- Another property with `AllowUpdates` set to `false`
- It also uses `@key`

In both of these cases, the **persisted value is not restored** upon page navigation