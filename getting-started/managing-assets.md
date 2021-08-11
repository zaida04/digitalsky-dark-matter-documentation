---
description: 'Learn how to create things like images, text, etc!'
---

# Managing Assets

## Getting to the Asset Manager

You can find the Asset Manager if it's not already open by going to the top bar,`Windows > Asset Manager` . You'll see a window that looks like this: 

![The Asset Manager](../.gitbook/assets/image%20%282%29.png)

We're going to quickly dissect this window so you know what each button does. The collection of folders on the left hand side are your folder of Assets \(`A6`\). There should be some that come with your copy of Dark Matter. You can create another one by clicking the the folder with a plus button in it \(`A1`\). Go ahead and give it a name and hit `OK`. You can now create assets in the folder by finding the folder in the folder list \(`A6`\) and clicking on it. You'll notice when you click on the folder once, `A6` doesn't change. But if you double click on it, `A6` turns into an "open folder" icon.

{% hint style="warning" %}
If the folder doesn't have the open icon, ASSETS CHANGED WILL NOT SAVE. 
{% endhint %}

{% hint style="warning" %}
If you click onto another folder, you must repeat this process to ensure that you always have an open folder icon like shown below, otherwise your changes won't save and you cannot create new assets.
{% endhint %}

![Closed folder icon](../.gitbook/assets/image%20%285%29.png)

![Open folder icon](../.gitbook/assets/image%20%283%29.png)

Now, onto creating the asset itself. If you see where `A5` is on the image above, that's where the different _types_ of assets are. The main types are slide and text for our purposes. 

![Slide and Text \(left and right\)](../.gitbook/assets/image%20%2810%29.png)

Let's start with the **slide** asset type. If you go ahead and click on it, you'll be prompted to give your new asset a name. **Note: You must have a folder selected to create an asset. The asset needs somewhere to go.** Once you go ahead and hit OK you'll notice that we have a new entry in the list under our various asset manager buttons. If you go ahead and click on it, you now have access to your very own asset. We will go over the various customization options for assets later. If you want to load an asset into a button, just click on the asset entry in the list that we talked about before, and drag it over to your button ScriptPad. This will make a line similar to: `Assets FolderName.Load(AssetName)` . You now have the button in your script ready to be used.



## Creating a Text Asset

Among the many types of Assets you can create in Dark Matter, the Text Asset is one of the most important ones. If you refer to the Asset Manager image above, if you scroll down `A5` you'll come across a T shaped icon, as shown in the figure below 

![Slide Asset \(left\) and Text Asset \(Right\)](../.gitbook/assets/image%20%2812%29.png)

If you click on the Text Asset, like all other assets, it'll prompt you for a title to give the asset and will allow you to hit Ok and create the asset.

{% hint style="warning" %}
You must have a folder selected for the asset to go to, if you don't have one selected then Dark Matter will NOT allow you to create the asset.
{% endhint %}

Once you have created your text asset, you'll see a new entry in the asset list in the folder you selected. From there you can look at the options on the right-hand side as depicted in the figure below. 

![Options for a Text Asset](../.gitbook/assets/image%20%2813%29.png)

From there, you can change the necessary settings for a text asset. One thing you'll most likely want to change is the `String` option, which is the text that is displayed. Inside that text box, go ahead and put in whatever you want your text to say. You can also change addition things like `text color`, `line spacing`, and more. You can change the positioning, rotation, and more of the text by changing the options under the `Apperance` tab. You now have a text asset usable in your project, just drag it into your scripts and you're ready to roll.

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

## How to create Video assets

Video assets are broken up into two parts. A **Media** asset and a **Slide** asset. The Media asset is what will contain the actual reference to the video file, while the Slide asset will just contain a reference to the Media asset. Think of the Slide asset as a canvas and the Media asset is just the actual art itself being put on the canvas. 

![Media asset](../.gitbook/assets/image%20%2816%29.png)

To create a Media asset, navigate to the Asset Manager and scroll down the Asset type list till you come across the Media asset type \(shown above\). From there, create it the same way you'd create other assets: assigning it a name and a folder destination. 

![Media asset configuration tab](../.gitbook/assets/image%20%2815%29.png)

Once you select your Media asset, you'll see the configuration tab on the right looks different from how the other Assets look. From there, you can customize the following properties \(and more\):

* **Looping -** Whether this asset will start from the beginning once it reaches the end.
* **File -** The path to the video/other media type file that will be connected to this Media asset.
* **Audio -** If your audio is separated from your video file \(i.e. gif\), then you can provide the path to your audio file.
* **Volume -** The volume in which the audio from your video or audio file will be played at.

Now that you have your Media asset all set up, you can go to the Slide asset that you created earlier. For the "picture" property of your Slide asset, place the following: \`Media:testVideoMedia\`. This text is broken up into two parts:  the "Media:" part that distinguishes to the Slide asset that you are not providing an actual file, but instead a reference to a Media asset, and the "testVideoMedia" part, which is just the name of the Media asset you are referencing.

Once you save both assets, you are ready to use them in your script. You must load in both the Slide asset and the Media asset. Your code will look something like this:

`Assets Stars-Spectrum.Load(testVideoMedia)` 

`Assets Stars-Spectrum.Load(testVideoSlide)` 

`+0.5`

`Scene testVideoSlide.Visibility=100` 

`Scene testVideoMedia.play()`

`Control text="Video over, let's continue!"`

`Control pause`

`Assets Stars-Spectrum.unload(testVideoMedia)` 

`Assets Stars-Spectrum.unload(testVideoSlide)`

Lines 1 & 2 load in the Media asset & the Slide asset. 

Line 3 is a delay we give to ensure the assets are loaded in time. 

line 5 is what starts the Media asset and plays it. 

Lines 6 & 7 change the button text and ensure that we're waiting until the video is done before we click to proceed.

Lines 8 & 9 unload the assets once you are done so you aren't using memory unnecessarily!

{% hint style="warning" %}
Remember to always save your assets once you are finished configuring them. Otherwise, you run the risk of losing your work!
{% endhint %}

