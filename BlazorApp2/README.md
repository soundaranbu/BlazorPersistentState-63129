# Blazor Persistent State Behavior

- The `Counter` page component uses a `PersistentState` attribute for the `currentCount` property.
    - The count persists and restores successfully on page load or refresh.
    - However, it does **NOT** restore when navigating between pages.

- The Home page uses a `CounterWithKey` component with two variations:
    - One property with `AllowUpdates` set to `true`.
    - Another property with `AllowUpdates` set to `false`.
    - It also uses the `@key` directive.

In both cases, the **persisted value is NOT restored** upon page navigation.