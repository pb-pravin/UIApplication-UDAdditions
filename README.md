UIApplicationStatusBarDidTouchNotification
=========

adds UIApplicationStatusBarDidTouchNotification. Did you ever wanted to implement some custom functionality then statysbar is touched?

Requirements
----------
iOS 3.0+

How To Use It
-------------
    #import "UIApplication+UDAdditions.h"
    ...

    [[UIApplication sharedApplication] registerForStatusBarTouchNotifications];
    
    [[NSNotificationCenter defaultCenter] addObserver: self
                                             selector: @selector(test)
                                                 name: UIApplicationStatusBarDidTouchNotification
                                               object: nil];