# How to disable ScrollViewer when DockingManager window containing MDI maximized document is resized?

In DockingManager, when an MDI maximized document is added and the MainWindow containing the DockingManager is resized, a ScrollViewer appears by default. This sample shows how to disable that ScrollViewer behavior by setting the `IsEnabledScroll` property of the `DocumentContainer` to `false`.

The DockingManager is configured with `UseDocumentContainer="True"` and `ContainerMode="MDI"`, and the document is added in document state. In the window constructor, the document container is accessed through the `DocContainer` property and its scrolling behavior is turned off. This prevents the automatic ScrollViewer from appearing when the maximized MDI document is resized along with the main window.

This approach is useful when you want a cleaner MDI document experience and do not want scrollbars to appear automatically during resize operations in WPF applications. It keeps the document area visually simple and easier to manage.
