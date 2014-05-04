UIlViewController+Tutorial
==================

Sources of UIlViewController+Tutorial and Demo app to show fancy on-boarding tutorials.

##Download
    $ git clone https://github.com/kronik/UIlViewController-Tutorial.git
    $ cd UIlViewController-Tutorial/

##Usage
Please check out the demo project included.
# ![Screenshot](https://raw.github.com/kronik/UIlViewController-Tutorial/master/example.gif)

### Initialization
``` objective-c

### Trigger navigation tutorial
``` objective-c
- (void)viewDidAppear: (BOOL)animated{
    [super viewDidAppear:animated];

    [viewController startNavigationTutorial];
}
```

### Trigger create new item tutorial
``` objective-c
- (void)viewDidAppear: (BOOL)animated{
    [super viewDidAppear:animated];

    [viewController startCreateNewItemTutorialWithInfo:NSLocalizedString(@"Pull down to create new item", nil)];
}
```

### Trigger tap to open settings tutorial
``` objective-c
- (void)viewDidAppear: (BOOL)animated{
    [super viewDidAppear:animated];

    [viewController startTapTutorialWithInfo:NSLocalizedString(@"Tap here to open settings", nil) 
                                     atPoint:CGPointMake(160, 350)
                        withFingerprintPoint:CGPointMake(160, 200) 
                        shouldHideBackground:NO];
}
```

##Requirements
Supported build target - iOS 7.x
Earliest supported deployment target - iOS 7.0

##License
UIlViewController+Tutorial is available under the MIT license. See the LICENSE file for more info.