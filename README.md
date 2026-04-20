# Disable ScrollViewer When an MDI‑Maximized DockingManager Document Is Resized

This sample demonstrates how to control scrolling behavior when using **Syncfusion WPF DockingManager** in **MDI mode** with a maximized document window. It shows how to prevent unwanted `ScrollViewer` behavior when the DockingManager window is resized while hosting a maximized MDI document.

## Overview
This example illustrates a scenario where DockingManager is configured to use a document container in MDI mode. When a document window is maximized, resizing the main window can cause an internal ScrollViewer to appear and affect the layout.

The sample demonstrates how to avoid this behavior by correctly configuring document sizing so that the document content adjusts itself without introducing scrollbars during resize operations.

## What This Sample Demonstrates
- How to use DockingManager in MDI document mode
- How to host document content using a ContentControl
- How to enable automatic size adjustment for document content
- How to avoid unwanted ScrollViewer behavior when resizing a maximized MDI document
- How to maintain a clean document layout during window resize operations

## Key Controls Used
- **DockingManager**: Manages document windows and layout in MDI mode
- **ContentControl**: Hosts document content within the DockingManager
- **Grid / Border**: Represents document content for visual clarity

## How It Works
1. DockingManager is configured to use a document container with `ContainerMode` set to `MDI`.
2. The document window is marked using `DockingManager.State="Document"`.
3. Automatic content sizing is enabled using `SizetoContentInDock`.
4. When the document is maximized, the content resizes along with the window.
5. This prevents ScrollViewer controls from appearing during window resizing.

## Benefits
- Prevents unwanted scrollbars during resize
- Improves user experience in MDI‑style applications
- Maintains consistent document layout behavior
- Ideal for document‑centric interfaces using DockingManager

This approach is useful for WPF applications that use DockingManager in MDI mode and require stable, scroll‑free resizing behavior for maximized document windows.