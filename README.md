Stacker is an iOS view-controller to kickstart development of hybrid native/web iOS apps. Stacker was built to keep your navigation native while the rest of your app is driven by webviews using [Stacker's special URLs.](http://www.lokimeyburg.com/Stacker/docs/url-structure/)

Built for: iPhones running iOS 7 & iOS 8 (iPad support coming soon)

## Features

- Build [URL-driven iOS apps](http://www.lokimeyburg.com/Stacker/docs/url-structure/)
- Send messages between Obj-C and JavaScript
- Custom navigation button handlers
- View external websites in a separate modal view
- Theming options
- Pull to refresh on all pages
- Error pages
- App version and device information sent in HTTP headers

## Getting Started & Documentation

[View the official Stacker documentation](http://www.lokimeyburg.com/Stacker/docs/getting-started/) to get started.

## Creating a StackerController

**If you're using [CocoaPods:](http://cocoapods.org)**

In your Podfile add:
```
pod 'LMStacker', :git => 'https://github.com/charlon/LMStacker.git'
```
And then run
```
$ pod install --no-clean
```

Now in your XCode project:

```
// Import Stacker
#import "LMStackerController.h"

// Create a controller and point it to your web app's url
LMStackerController *myController = [[LMStackerController alloc] initWithURL:@"http://localhost:3000?x_page_title=Home"];
```
