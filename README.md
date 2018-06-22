# UseIQKeyboardManager
Handle Keyboard   

[github地址](https://github.com/hackiftekhar/IQKeyboardManager)

## Step1  
* 1 pod 'IQKeyboardManager'


* 2 使用 #import <IQKeyboardManager.h>

```- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions {
	// Override point for customization after application launch.
	 IQKeyboardManager *keyboardManager = [IQKeyboardManager sharedManager]; // 获取类库的单例变量
	// 启动键盘管理功能
	keyboardManager.enable = YES;
	// 点击空白处关闭键盘
	keyboardManager.shouldResignOnTouchOutside = YES;
	// 控制是否显示键盘的工具条
	keyboardManager.enableAutoToolbar = YES;
	// 输入框距离键盘的距离
	keyboardManager.keyboardDistanceFromTextField = 40.0f;
	
	return YES;
}
```
