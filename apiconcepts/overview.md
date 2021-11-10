# MultiTerm Desktop SDK #
The Software Development Kit (SDK) contains an introduction to the MultiTerm Client API as well as a full programming reference. It contains various practical examples of how to implement functionality into third-party party applications and custom workflows. 

## Introduction

This Software Development Kit (SDK) contains an introduction to the MultiTerm Client API as well as a full programming reference. It contains various practical examples of how to implement functionality into third-party party applications and custom workflows.

## In this version of the MultiTerm SDK, the following APIs are documented:
This enables you, for example, to make the MultiTerm lookup and editing functionality available directly from within various applications or document management/authoring systems.

| <!----> | <!----> | <!----> | <!----> |
| --- | --- | --- | --- |
| **Component** | **MultiTerm version** | **API Version** | **Main Class** |
| TRADOS MultiTerm 16.0 Client API | 2021 SR2 | 11.0 | Sdl.MultiTerm.TMO.Interop.Application (C#)<br> MultiTermIX (VBA) |


The corresponding DLL library can be found in your SDL Common Files installation folder, e.g.: *C:\Program Files (x86)\Common Files\SDL\MultiTerm16\Sdl.MultiTerm.TMO.dll*

The interop dll for use in C# can be found in the same folder, e.g.: *C:\Program Files (x86)\Common Files\SDL\MultiTerm16\Sdl.MultiTerm.TMO.Interop.dll*

For use in VBA, reference the COM component **MultiTerm.TMO**

## Conventions

Names of objects, classes, methods, properties, events and settings are formatted in bold. Example: "Use **Sdl.MultiTerm.TMO.Interop.Application** to create a new MultiTerm client instance."

Sample code is formatted in Courier and is separated from the body text. Example:

```cs
Termbase.SourceIndex =
Termbase.Definition.Indexes.Item("English")
```
All sample code in this guide is provided in Microsoft C#.

## Other information resources

[RWS Software Development Kit](https://developers.rws.com/)

[RWS products](https://www.rws.com/contact/product-enquiry/)


## SDK Support

Please note that the SDK is provided as is and for use at your own risk. RWS does not provide support and consulting services unless expressly agreed upon in a Support & Maintenance contract.

[Legal notice](LegalNotice.md)

Copyright and trademark information relating to this product release.

[Acknowledgments](Acknowledgments.md)

MultiTerm includes open source or similar third-party software.
