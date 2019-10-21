---
title: Getting the Units of the Active Document
description: This brief guide demonstrates how to determine the unit system of the active document.
authors: ['dale_fugier']
sdk: ['C/C++']
languages: ['C/C++']
platforms: ['Windows']
categories: ['Fundamentals']
origin: http://wiki.mcneel.com/developer/sdksamples/unitsystem
order: 1
keywords: ['rhino', 'units', 'document']
layout: toc-guide-page
---

 
## Overview

There are two unit systems associated with a document, model and page units. The `ON_UnitSystem` class makes it easy to work with custom units. The Rhino document class contains two functions to return these unit systems:

1. `const ON_UnitSystem& CRhinoDoc::ModelUnits() const;`
1. `const ON_UnitSystem& CRhinoDoc::PageUnits() const;`

## More information

The unit system of the active document is stored on an `ON_3dmUnitsAndTolerances` class that is located on the `CRhinoDoc` object.

If you inside of a `CRhinoCommand`-derived object's `RunCommand()` member, you can get the current units system as follows:

```cpp
const CRhinoDocProperties& doc_props = context.m_doc.Properties();
const ON_3dmUnitsAndTolerances& units_tolerances = doc_props.ModelUnitsAndTolerances();
ON::LengthUnitSystem units_system = units_tolerances.m_unit_system;
```

As a shortcut, you can do the following:

```cpp
ON::LengthUnitSystem units_system = context.m_doc.UnitSystem();
```

If you outside of a `CRhinoCommand`-derived object's `RunCommand()` member, you can get the current units system as follows:

```cpp
CRhinoDoc* doc = RhinoApp().ActiveDoc();
if (nullptr != doc)
{
  ON::LengthUnitSystem units_system = doc->UnitSystem();
}
```
