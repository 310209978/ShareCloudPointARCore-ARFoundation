# ShareCloudPointARCore-ARFoundation

In this demo you can share the same cloud point with your partener who use the same demo.</br>

Use: ARCore and ARFoundation</br>

Testing this app</br>
When you run your app you can test the basic behavior as follows:</br>

Holding your device, move around your space, slowly scanning an area you would like to host a new Cloud Reference Point from. Try to collect at least 10 seconds of data, and scan the area from several directions before moving to the next step. You should see feature points and detected planes render on your screen.</br>
Tap on the screen to create a new Cloud Reference Point. Selecting a point near interesting features, as opposed to empty space or blank walls will generally yield better results. (If you connected the LocalReferencePoint prefab to your AR Reference Point Manager, you will see it appear at the location.)</br>
Wait for the new Cloud Reference Point to be ready. The HostedPoint prefab (a blue sphere) will appear at the location when it is ready to use, and the Cloud Reference Id will be displayed in the text field at the bottom of your screen.</br>
Again scan around the area with the reference point for at least 10 seconds, then tap the screen again to resolve the current point. (This will ultimately make two copies of the same point, but it demonstrates the flow in code you will use when you receive the Cloud Reference Id from another client using your app.)</br>
Wait for the new Cloud Reference Point to be ready. When it is resolved and ready, another LocalReferencePoint prefab (yellow cube) will appear coinciding with the ResolvedPoint prefab (red cylinder). This second local Reference Point will not appear in future versions of AR Foundation.</br>
You may repeat the process to create another Cloud Reference Point in step 1, or...
Obtain a Cloud Reference Id from another device (run the app on a second device) and enter the Id into the text input field on the first device.</br>
Wait as you did in step 5 until the corresponding Cloud Reference Point is created and ready to use.</br>



