---
description: How to create and manage your assets
---

# Assets

Assets are the forefront to creating media using Digital Sky Dark Matter. They are managed through the **Asset Manager,** which is where you can create and see a list of all your Assets.

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

