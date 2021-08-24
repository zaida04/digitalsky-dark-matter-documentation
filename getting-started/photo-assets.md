# Photo Assets



## How to make a Slide Asset \(Image\)

The steps to making a Slide Asset are almost identical to the Text Asset portion. Because it is also an asset you will most likely be making, we're going to go over it. Scroll to the same area you saw the Text Asset icon at in `A5` \(if you don't remember where this is, refer to the figure regarding it in the above section\). Directly on the other side of the Text Asset icon, there is the Slide Asset icon. Go ahead and create it with the same steps the Text Asset took. 

![Slide Asset options](../.gitbook/assets/image%20%2814%29.png)

Now the major part here is selecting the path to the image you want connected to this slide. Under the `Appearance` tab, you'll notice the `Picture` option, go ahead and click the empty button next to the path, and it'll direct you to navigate to the media you want to use with this asset. Once you've chosen your asset, you'll notice the text in `Picture` has changed to the path leading to your media. You now have a slide asset that you can use in your projects just like how you use the other assets.

## How to customize Slide assets

![Random asset&apos;s appearance settings](../.gitbook/assets/zoom_obuotg3zhm.png)

All slides allow you to customize how they look on the screen, things like size, position, and more are easily configurable through the Appearance tab. You can find the Appearance tab by scrolling down the list that'll open up on the right hand side \(that looks like the above image\) when you select an asset in the asset manager. From there, you can customize the following:

* **Visibility -** The opacity of your slide, 0% meaning your slide is not visible, 100% meaning your slide is entirely visible and is not transparent at all. Useful for "visibility transitions".
* **Picture -** The path to the image/media that your slide will display. Can be anchored to Media type assets \(e.x. Media:testVideoMedia\).
* **Azimuth -** How far east or west an asset will go, the equivalent of moving it left or right on the dome.
* **Elevation -** How far up or down an asset will go facing towards the center. This setting is impacted by your azimuth, as it won't just plainly go up and down the y-axis.  
* **Rotation -** The rotation of your asset out of 360 degrees.
* **Width -** The width of the asset
* **Height -** The height of the asset
* **Lock -** Whether or not the width and height are locked. Commonly referred to as an "Aspect Ratio lock".

## How to use Image Assets in your buttons

Once you have an asset created, it is as simple as:

* Open the Button script up
* Click on the Asset you wish to load
* Drag the Asset name all the way to the script text area
* Let go and watch the code be auto-generated for you

![Photo version of the above steps](../.gitbook/assets/image%20%2821%29.png)

Once you do that, there should be a new code snippet in your Script tab looking something like this:

![The snippet generated will be like this: &quot;Assets YOUR\_ASSET\_FOLDER\_NAME.Load\(YOUR\_ASSET\_NAME\)&quot;](../.gitbook/assets/image%20%2820%29.png)

These same steps can be done for the properties of a slide, like Visibility. Say, for example you'd like to hardcode the starting value of your Slide Asset to 100, you would repeat the above steps but click on the actual property you want to drag over -- as shown below.

![Photo version of where you&apos;d click and where you&apos;d drag to](../.gitbook/assets/image%20%2818%29.png)

![The generated code snippet](../.gitbook/assets/image%20%2819%29.png)

As you can see, manual coding isn't needed entirely throughout Dark Matter, you can have the application generate the code for your Button scripts most of the time.

{% hint style="warning" %}
Remember to always save your assets once you are finished configuring them. Otherwise, you run the risk of losing your work!
{% endhint %}

