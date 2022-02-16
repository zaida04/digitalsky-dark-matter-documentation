# Video Assets

## How to do Regular Video

Video assets are broken up into two parts. A **Media** asset and a **Slide** asset. The Media asset is what will contain the actual reference to the video file, while the Slide asset will just contain a reference to the Media asset. Think of the Slide asset as a canvas and the Media asset is just the actual art itself being put on the canvas.&#x20;

![Media asset](<../.gitbook/assets/image (16).png>)

To create a Media asset, navigate to the Asset Manager and scroll down the Asset type list till you come across the Media asset type (shown above). From there, create it the same way you'd create other assets: assigning it a name and a folder destination.&#x20;

![Media asset configuration tab](<../.gitbook/assets/image (15).png>)

Once you select your Media asset, you'll see the configuration tab on the right looks different from how the other Assets look. From there, you can customize the following properties (and more):

* **Looping -** Whether this asset will start from the beginning once it reaches the end.
* **File -** The path to the video/other media type file that will be connected to this Media asset.
* **Audio -** If your audio is separated from your video file (i.e. gif), then you can provide the path to your audio file.
* **Volume -** The volume in which the audio from your video or audio file will be played at.

Now that you have your Media asset all set up, you can go to the Slide asset that you created earlier. For the "picture" property of your Slide asset, place the following: \`Media:testVideoMedia\`. This text is broken up into two parts:  the "Media:" part that distinguishes to the Slide asset that you are not providing an actual file, but instead a reference to a Media asset, and the "testVideoMedia" part, which is just the name of the Media asset you are referencing.

Once you save both assets, you are ready to use them in your script. You must load in both the Slide asset and the Media asset. Your code will look something like this:

```
Assets YOUR_FOLDER_NAME.Load(YOUR_MEDIA_ASSET) 
Assets YOUR_FOLDER_NAME.Load(YOUR_SLIDE_ASSET) 
+0.5
Scene YOUR_SLIDE_ASSET.Visibility=100 
Scene YOUR_MEDIA_ASSET.play()
Control text="Video over, let's continue!"
Control pause
Assets YOUR_FOLDER_NAME.unload(YOUR_MEDIA_ASSET) 
Assets YOUR_FOLDER_NAME.unload(YOUR_SLIDE_ASSET)
```

Lines 1 & 2 load in the Media asset & the Slide asset.&#x20;

Line 3 is a delay we give to ensure the assets are loaded in time.&#x20;

line 5 is what starts the Media asset and plays it.&#x20;

Lines 6 & 7 change the button text and ensure that we're waiting until the video is done before we click to proceed.

Lines 8 & 9 unload the assets once you are done so you aren't using memory unnecessarily!

## How to do Full Dome Video

Full dome video steps are similar to the above regular video steps. The only step you'd remove is creating and editing the Slide asset that you would create connected to your Media asset. There is a Global Asset meant to be used with Full Dome video, so you'd simply write the following code:

{% hint style="danger" %}
When you create the media asset and select the MPG and DSI file from the file picker, you will most likely have a path that includes a number at the end. **You need to replace that number with a wildcard "\*" or the video will not be full dome.**\
****\
****Example: `E:\DigitalSkyDM\Modules\Skyvision\ClipsDemos\ESO-CMEandEarth_01.mpg`

Transformed:&#x20;

`E:\DigitalSkyDM\Modules\Skyvision\ClipsDemos\ESO-CMEandEarth_*.mpg`
{% endhint %}

```
Assets YOUR_ASSET_FOLDER.Load(YOUR_MEDIA_ASSET)
+1
Scene Video.Source="Media:YOUR_MEDIA_ASSET"
Scene YOUR_MEDIA_ASSET.Play()
+1
Scene Camera.Visibility=0 [1]
Scene Video.Visibility=100 [1]
Control Pause
+1
Scene Camera.Visibility=100 [1]
Scene Video.Visibility=0 [1]
+1
Assets YOUR_ASSET_FOLDER.Unload(YOUR_MEDIA_ASSET)
```

The following code loads in your Media asset, starts it, then sets the Global Video Asset used for Full Dome Video (Video.Source) to your Media asset. Once the video is done playing, you can press the button again and it'll unload the Media asset.&#x20;

{% hint style="warning" %}
Remember to always save your assets once you are finished configuring them. Otherwise, you run the risk of losing your work!
{% endhint %}
