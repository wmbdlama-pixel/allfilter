# AllFilter

**Filter, select, hide or isolate Revit elements by category, type and parameter value —
including text notes by their content and tags by the text they display.**

AllFilter is an add-in for Autodesk Revit, published by **wmbdlama**.

---

## What it does

AllFilter builds a live **Category → Parameter → Value** tree from your current selection,
or from the whole model when nothing is selected. Tick the values you care about, then
select, hide, isolate or reveal the matching elements.

- Three-level tree with the element count next to every value.
- Instance and type parameters side by side; type parameters are marked `[TYPE]`.
- Empty values are a first-class target: ticking `<EMPTY>` finds everything where a
  parameter was never filled in.
- **Text notes** can be filtered by their actual text content.
- **Tags** can be filtered by the text shown on the tag — including room tags, space tags
  and area tags, which belong to a different class in Revit and are normally missed.
- Parameter search, and Shift-click to tick a whole range of values at once.
- Values inside one parameter combine with OR; different parameters combine with AND.

The tree loads lazily, so large models open without a wait. The window is modeless: you
can keep working in Revit while it is open.

**Nothing in your model is modified.** AllFilter only selects elements and changes
temporary view visibility, both of which Revit can undo.

---

## Supported versions

| Revit | Platform |
|---|---|
| 2023, 2024 | .NET Framework 4.8 |
| 2025, 2026 | .NET 8 |
| 2027 | .NET 10 |

Windows 10 or Windows 11, 64-bit. No internet connection is required to use AllFilter.

---

## Documentation

- [How to use AllFilter](HELP.md)
- [Privacy policy](PRIVACY.md)

---

## Support

Questions, bug reports and feature requests: **wmbdlama@gmail.com**

Please include your Revit version and build, a short description of what you expected and
what happened instead, and a screenshot if the problem is visible on screen. Emails are
answered within two business days, Monday to Friday.

---

© 2026 wmbdlama
