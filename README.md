# How to disable ScrollViewer when DockingManager window containing MDI maximized document is resized?
In DockingManager when MDI maximized document are added and MainWindow containing DockingManager is resized, the ScrollViewer appears by default. This ScrollViewer can be disabled by setting IsEnabledScroll property value as false.

## C#
    // To disable ScrollViewer for MDI maximized document
    (TheDocker.DocContainer as DocumentContainer).IsEnabledScroll = false;
## VB
    ' To disable ScrollViewer for MDI maximized document
     TryCast(TheDocker.DocContainer, DocumentContainer).IsEnabledScroll = False
