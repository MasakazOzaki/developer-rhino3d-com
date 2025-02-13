---
title: What is RhinoMobile?
description: This guide gives and overview of RhinoMobile.
authors: ['dan_rigdon_bel']
sdk: ['RhinoMobile']
languages: ['C#']
platforms: ['iOS', 'Android']
categories: ['Overview']
origin: http://wiki.mcneel.com/developer/rhinomobile
order: 1
keywords: ['RhinoMobile', 'iRhino 3D']
layout: toc-guide-page
---

 
![{{ site.baseurl }}/images/rhinomobile-overview-01.png]({{ site.baseurl }}/images/rhinomobile-overview-01.png){: .float-img-right width="325"}

RhinoMobile is a C# .NET library for the development of 3D, cross-platform, mobile applications. RhinoMobile - like RhinoCommon - is based on the Xamarin Mono framework, a fully-functional .NET runtime that works on Android, iOS and macOS. RhinoMobile uses openNURBS (the 3dm NURBS library) and RhinoCommon (the .NET SDK for Rhinoceros and Grasshopper) and handles file IO, gesture recognition and 3D display (OpenGL ES 2.0). It's not the entirety of RhinoCommon, but a subset.

## Who should use it?

Anyone interested in developing, prototyping, or just experimenting with 3D mobile development. Though there are many good 3D libraries out there for mobile games, none are focused on 3D modeling and design. RhinoMobile seeks to fill that gap. If you want to develop in C# and target as many devices as possible, this is the library for you. No experience with mobile development necessary...just familiarity with C# and .NET.

## Where can I get help?
{: .clear-img}
Visit the [Rhino Forum](http://discourse.mcneel.com/) and post your question in the [Rhino Developer Category](http://discourse.mcneel.com/c/rhino-developer) and @mention the developer @dan.

## Downloads & Links

### Developer Tools

- [Xamarin Platform](http://xamarin.com/download). Using RhinoMobile requires a 30-day free trial of the Business Edition. - Xamarin does have reduced academic pricing.
- [Xcode](http://developer.apple.com/xcode/) on a Mac running OS X 10.8 (Mountain Lion) or greater for building iOS apps.
- [Visual Studio 2012](http://https//www.visualstudio.com/en-us/visual-studio-homepage-vs.aspx) or better: Non-Express editions only (Xamarin's extensions require paid versions).
- [Intel Hardware Accelerated Execution Manager](http://software.intel.com/en-us/articles/intel-hardware-accelerated-execution-manager/) provides hardware-acceleration for Android emulators.

### Libraries & Samples

- [RhinoCommon (rhino3dmio branch)](https://github.com/mcneel/rhinocommon/tree/rhino3dmio): The .NET plugin SDK for Rhino and Grasshopper.
- [openNURBS](http://www.rhino3d.com/opennurbs) Download: C++ openNURBS SDK.
- [RhinoMobile](http://github.com/mcneel/RhinoMobile) Download or clone the RhinoMobile library.
- [RhinoMobileSamples](http://github.com/mcneel/RhinoMobileSamples) Download or clone some sample projects that use RhinoMobile.

---

## FAQ

**Is RhinoMobile free?**

Yes.

**Can I sell the apps I develop with RhinoMobile?**

Yes.

**Will apps build with RhinoMobile work on Mac and Windows computers as well as mobile devices?**

No, with one caveat: though we have yet to add it to the library, we plan on supporting Windows Phone, which uses a DirectX as a display pipeline and can be run (with some limitations) as a “Windows Store App” (aka: Metro UI app).

**Does McNeel use RhinoMobile to develop iRhino 3D?**

We sure do.

**Wait, is this all of RhinoCommon?**

No. RhinoMobile uses a subset of RhinoCommon (rhino3dmio), the limits of which are defined by the symbol: MOBILE_BUILD. There's a lot there: Rhino.DocObjects, Rhino.Geometry, Rhino.FileIO...pretty much everything you'd need to read, write, and draw Rhino 3dm.

**So I probably can't perform Meshing or run a Make2D command?**

Sorry, not yet. Given the CPU constraints of mobile platforms, you'd probably consume all your battery life doing so anyway.

---

## Next Steps

If you are ready to get started with RhinoMobile, begin by making sure you have all the tools installed.  Read:

- [Installing Tools (Mac)]({{ site.baseurl }}/guides/rhinomobile/installing-tools-mac/); or
- [Installing Tools (Windows)]({{ site.baseurl }}/guides/rhinomobile/installing-tools-windows/)

---

## Related Topics

- [What is RhinoCommon?]({{ site.baseurl }}/guides/rhinocommon/what-is-rhinocommon/)
- [What are Mono & Xamarin?]({{ site.baseurl }}/guides/rhinocommon/what-are-mono-and-xamarin/)
- [Installing Tools (Mac)]({{ site.baseurl }}/guides/rhinomobile/installing-tools-mac/)
- [Installing Tools (Windows)]({{ site.baseurl }}/guides/rhinomobile/installing-tools-windows/)
