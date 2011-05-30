---
layout: project
title: Android Smart Image View
tagline: Load Images from URLs or Android Contacts with Caching
version: 1.0.0
github_url: https://github.com/loopj/android-smart-image-view
download_url: https://github.com/loopj/android-smart-image-view/zipball/android-smart-image-view-1.0.0.jar
---


Overview
--------
`SmartImageView` is a drop-in replacement for Android's standard `ImageView`
which additionally allows images to be loaded from URLs or the user's contact
address book. Images are cached to memory and to disk for super fast loading.


Features
--------
- Drop-in replacement for `ImageView`
- Load images from a URL
- Load images from the phone's contact address book
- Images are cached to memory and to disk for super fast loading
- `SmartImage` class is easily extendable to load from other sources


Installation & Basic Usage
--------------------------
Download the latest .jar file from github and place it in your Android app's
`libs/` folder.

Add a `SmartImageView` to your activity's xml layout:
{% highlight xml %}
<com.loopj.android.image.SmartImageView
    android:id="@+id/my_image" />
{% endhighlight %}

Get a reference to the layout's `SmartImageView`:
{% highlight java %}
SmartImageView myImage = (SmartImageView) this.findViewById(R.id.my_image);
{% endhighlight %}

Load an image into the view from a URL:
{% highlight java %}
myImage.setImageUrl("http://www.awesomeimages.com/myawesomeimage.jpg");
{% endhighlight %}

Load an image into the view from the phone's contact address book:
{% highlight java %}
myImage.setImageUrl(contactAddressBookId);
{% endhighlight %}


Reporting Bugs or Feature Requests
----------------------------------
Please report any bugs or feature requests on the github issues page for this
project here:

<https://github.com/loopj/android-smart-image-view/issues>


License
-------
The Android Smart Image View is released under the Android-friendly
Apache License, Version 2.0. Read the full license here:

<http://www.apache.org/licenses/LICENSE-2.0>
