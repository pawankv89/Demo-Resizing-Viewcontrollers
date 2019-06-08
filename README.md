
Demo Resizing Viewcontrollers
=========

## Demo Resizing Viewcontrollers.
------------
 Added Some screens here.
 
![](https://github.com/pawankv89/DemoResizing/blob/master/Screens/1.png)
![](https://github.com/pawankv89/DemoResizing/blob/master/Screens/2.png)

## Usage
------------
 iOS 9 Demo showing how to Demo Resizing Viewcontrollers on iPhone X Simulator in  Objective-C.

```Swift
class ViewController: UIViewController {

override func viewDidLoad() {
super.viewDidLoad()
// Do any additional setup after loading the view, typically from a nib.
let popUpHsn:SecondViewController = self.storyboard?.instantiateViewController(withIdentifier: "SecondViewController") as! SecondViewController

//Add Chield ViewController with Custom Frame
self.addChildViewController(popUpHsn)
self.view.addSubview(popUpHsn.view)
popUpHsn.view.frame = self.view.frame
popUpHsn.didMove(toParentViewController: self)

//Resize Main ViewController
popUpHsn.view.frame = CGRect(x: 10, y: 70, width:300, height: 300) //Change Your Main ViewController Frame
popUpHsn.view.center = self.view.center// Add in Last

//Resize View in Side View
//popUpHsn.views.frame = CGRect(x: 20, y: 136, width:200, height: 200) //Change Your Main ViewController Frame
//popUpHsn.views.center = self.view.center// Add in Last

}

override func didReceiveMemoryWarning() {
super.didReceiveMemoryWarning()
// Dispose of any resources that can be recreated.
}


}


```

```objective-c


```

```objective-c

```

## License

This code is distributed under the terms and conditions of the [MIT license](LICENSE).

## Change-log

A brief summary of each this release can be found in the [CHANGELOG](CHANGELOG.mdown). 
