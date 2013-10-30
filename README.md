Quick start:

1. Install [CocoaPods](http://cocoapods.org/) with `gem install cocoapods`.
2. Create a file in your XCode project called `Podfile` and add the following line:
```
pod 'Mixpanel'
```
3. Run `pod install` in your xcode project directory. CocoaPods should download and
install the Mixpanel library, and create a new Xcode workspace. Open up this workspace in Xcode.
4. Add the following to your `AppDelegate.m`:
```Objective-C
#import <Mixpanel/Mixpanel.h>

- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions {
    [Mixpanel sharedInstanceWithToken:MIXPANEL_TOKEN];
}
```
5. Track an event in your application:
```Objective-C
    [[Mixpanel sharedInstance] track:@"Clicked Button"];
```

**Check out the [full documentation](https://mixpanel.com/help/reference/ios) →**
