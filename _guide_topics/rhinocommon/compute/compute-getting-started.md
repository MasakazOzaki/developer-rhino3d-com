---
title: Rhino Compute &trade;
description: This guide covers the tools required to get started with the Rhino Compute Service.
authors: ['steve_baer', 'scott_davidson']
sdk: ['RhinoCommon', 'Compute']
languages: ['C#', 'JavaScript', 'Python']
platforms: ['Windows', 'Mac']
categories: ['Getting Started']
origin:
order: 1
keywords: ['first', 'RhinoCommon', 'Plugin', 'compute']
layout: toc-guide-page
---

Compute is an open-source online advanced geometry extension as a web product based on Rhinoceros 3d's RhinoCommon API. The Compute is a compliment the Rhino3dm Geometry library. See the [Compute website](https://www.rhino3d.com/compute) for more overview information.

Compute can be accessed from CPython, JavaScript and C# (.NET).  It runs on many platforms including Windows, OSX, IOS, Unix, All major browsers and Node.JS.

---

## Setting up a Compute Project

There are a few tools which are essential to communicate with the Compute server. Select one of the supported languages:

- [Python]({{ site.baseurl }}/guides/rhinocommon/compute/compute-python-getting-started/) -  The CPython wrapper for [OpenNurbs]({{ site.baseurl }}/guides/opennurbs/) which contains the functions to read and write Rhino Geometry Objects. This is available as a Pip package.
- [JavaScript]({{ site.baseurl }}/guides/rhinocommon/compute/compute-javascript-getting-started) - The Javascript library and web assembly (WASM) to access Compute through any major browser or Node JS.
- [C# (.NET)]({{ site.baseurl }}/guides/rhinocommon/compute/compute-net-getting-started) - The nuget packages required to access to the Rhino3dm and Compute API.

## Support

The libraries are still very new and changing rapidly. Give them a try or get involved. Ask any questions or share what you are working on the [Compute Discussion Forum](https://discourse.mcneel.com/c/serengeti/compute-rhino3d)
