---
# required metadata

title: Visual Studio 2017 requirements for X++
description: This topic lists the Visual Studio 2017 components that are required to run the Visual Studio extension for X++.
author: jorisdg
ms.date: 04/01/2021
ms.topic: article
audience: Developer
ms.reviewer: rhaertle
ms.author: jorisde
ms.search.validFrom: 2020-04-01
ms.dyn365.ops.version: AX 7.0.0

---

# Visual Studio 2017 requirements for X++

[!include [banner](../includes/banner.md)]

This topic lists the Visual Studio 2017 components that are required to run the **Visual Studio** extension for X++.

> [!NOTE]
> We do not recommend installing Visual Studio manually on the downloadable virtual hard drive (VHD) or virtual machines deployed from Lifecycle Services (LCS). Instead, we strongly recommend that you download or deploy a new virtual machine. Virtual machines deployed with versions 10.0.13 or later all have Visual Studio 2017 and its prerequisites installed, and come with other updates outside of Visual Studio to help keep the machines compatible and secure.

## Visual Studio editions

The supported editions of Visual Studio include:

- Visual Studio 2017 Professional
- Visual Studio 2017 Enterprise

> [!NOTE]
> Different Visual Studio editions have different licensing requirements and costs. For more information, see [Visual Studio](https://visualstudio.microsoft.com).

## Required Visual Studio components

The following table lists the required Visual Studio components.

| Type | Name | Required | Notes |
| --- | --- | --- | --- |
| Workload | .NET desktop development | Yes | |
| Individual component | Modeling SDK | Yes | |
| Individual component | Directed Graph Markup Language (.dgml) editor | No | This component is used for dependency graph features. |
| Visual Studio Marketplace | Microsoft Reporting Services Projects | Yes | This component is needed for report development. If the component isn't installed, Visual Studio will prompt you when you try to open report designs. |

## Dynamics 365 Commerce

For more information on Commerce and Visual Studio 2017, see these topics.

- [Migrate the Retail SDK from Visual Studio 2015 to Visual Studio 2017](../../../commerce/dev-itpro/retail-sdk/migrate-sdk.md)
- [Development and ALM changes from version 10.0.10 to 10.0.13](../../../commerce/dev-itpro/dev-changes-10-13.md)
