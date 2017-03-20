# Rotation Issue

To reproduce the issue.  Run this project in the simulator.  Select an iPad as the device.  I've been using iPad 2.  When the device loads, you will see 10 black cells in the detail view.  Rotate the device.  Notice that the padding around the cells isn't the same.  Click the plus button to create a row on the master view.  When you click that new row, the detail view is recreated and the padding is correct.

According to the documentation, the collection view should automatically respond to changes in rotation.  I've tried invalidating the layout when rotation is detected, but it doesn't fix the layout issue.  Why doesn't the UICollectionViewDelegateFlowLayout keep the layout correct after rotation?  
