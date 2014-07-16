swift-async-image-cache
=======================

A simple library for iOS developing using Swift, it is an async image loading and local file-based cache extension for UIImageView. Any fork or star will be appreciated.

The project is written as an extension of UIImageView, it covers most of the use of image cache system. Sure, you can edit it with your own purpose.

How to use
=======================
<pre>
class UIIndexViewController : UIViewController {
  @IBOutlet var demoImageView : UIImageView
  // let`s pretent the demoImageView is linked to an UIImageView element in storyboard
  override func viewDidLoad() {
    super.viewDidLoad()
    demoImageView.loadImage("https://github.com/images/modules/dashboard/bootcamp/octocat_repo.png", autoCache: true)
  }
}
</pre>
Custom cache
=======================
You can easily change the second argument (autoCache) to false to force update local cache, if you set autoCache: true, the extension will not update the cache with same URL until you delete the cache.

Custom cache expire time will be added in the future.

Contact me
=======================
Feel free to contact me <me@idickyt.com>, or you can directly fork this project.
