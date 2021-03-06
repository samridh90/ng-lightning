Dropdowns offer items that the user can choose from.

Add the `nglDropdown` directive to the `<div>` that wraps the dropdown list.

Use the `nglDropdownTrigger` directive to any child element,
usually a `<button>` or a `<a>`, to open or close the dropdown.

Add the `nglDropdownItem` directive on any child element that constitutes
a dropdown item.

You can easily create a picklist just by combining the `<ngl-picklist>` with the `nglPick` directive.

When using the `ngl-picklist` component you can use the `filter` attribute to
set a filtering method for the items. The available options are a `string`,
which is taken to be a property or each item's backing object, a user provided
`function` to be used for filtering or no value at all. In the latter case,
each item is assumed to provide an implementation of the `toString` method.

**Accessibility and Keyboard interactions**:

  * `Space` and `Enter` on an `nglDropdownTrigger` toggle the dropdown's open status
  * `DownArrow` on an `nglDropdownTrigger` opens the dropdown and moves focus to the first dropdown item
  * An open `nglDropdown` has `aria-selected="true"` and a closed one has `aria-selected="false"`
  * `DownArrow` and `UpArrow` on an open `nglDropdown` move focus to the next and previous items respectively
  * `Escape` closes an open `nglDropdown` and moves focus to the `nglDropdownTrigger`
  * `Tab` closes an open `nglDropdown` and moves focus to the next focusable element
