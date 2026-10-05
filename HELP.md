# AllFilter — Help

Filter, select, hide or isolate Revit elements by category, type and parameter value —
including text notes by their content and tags by the text they display.

---

## Starting the add-in

Open a model, then on the **Add-Ins** tab click **All Filter**.

If elements are selected when you start it, AllFilter works on that selection. If nothing
is selected, it works on the whole model. Starting with a selection keeps the tree small
and every step faster.

With the pointer over the **All Filter** button on the ribbon, pressing **F1** opens this
page.

---

## Building a filter

1. Expand a category in the left tree to see its parameters.
2. Expand a parameter to see its values. The number next to each value is how many elements
   carry it.
3. Tick the values you want. They appear in the right tree, which shows the filter you have
   built so far.

Ticking a category itself takes every element in that category. A category and individual
values inside it are mutually exclusive — ticking one clears the other, because the two
would contradict each other.

---

## How values combine

| | |
|---|---|
| **Within one parameter** | **OR** — an element matches if it has any of the ticked values. |
| **Between parameters** | **AND** — an element must match every parameter you filtered on. |

---

## Reading the tree

| Marker | Meaning |
|---|---|
| `[TYPE]` | A type parameter. Without the prefix it is an instance parameter. |
| `<EMPTY>` | The parameter is empty or absent on those elements. Ticking it finds everything that was never filled in. |
| `[ReadOnly]` | The value comes from a parameter Revit does not allow you to edit. |
| `Text content` | Available on text notes: the text itself becomes a filterable value. |
| `Tag Text` | Available on tags: the text shown on the tag. Works for regular tags and for room, space and area tags. |
| `[42]` | How many elements carry that value. |

---

## Shortcuts

| | |
|---|---|
| **Search box** | Narrows the parameter list. `Enter` applies, `Esc` clears. |
| **Shift + click** | Ticks or unticks a whole range of neighbouring values at once. |
| **Reset** | Clears the search and the filter and rebuilds the tree. |
| **About** | Shows the version, the support address and the full privacy policy. |

---

## Actions

| | |
|---|---|
| **Select** | Selects the matching elements in the model. |
| **Hide** | Temporarily hides them in the active view. |
| **Isolate** | Temporarily isolates them in the active view. |
| **Show in model** | Reveals and zooms to them, opening a suitable view if needed. |

The window closes once the action is handed to Revit. Clear a temporary hide or isolate
with Revit's own **Reset Temporary Hide/Isolate** button on the view control bar.

---

## If something does not work

**Hide and Isolate report that the view does not support them.**
The active view is a schedule, sheet or legend. Switch to a plan, section, elevation or 3D
view.

**A parameter is missing from the tree.**
The tree lists parameters found on the elements in scope. If the parameter exists only on
elements outside your selection, start AllFilter with nothing selected so it reads the
whole model.

**Nothing matches a value you can see in the tree.**
Values are matched as the text Revit displays. If the same number is formatted differently
on different elements, Revit reports them as different values.

---

## Support

**wmbdlama@gmail.com** — answered within two business days, Monday to Friday.

Please include your Revit version and build, what you expected, what happened instead, and
a screenshot if the problem is visible on screen.

---

AllFilter 1.0.0 — Revit 2023, 2024, 2025, 2026, 2027
[Privacy policy](PRIVACY.md) · © 2026 wmbdlama
