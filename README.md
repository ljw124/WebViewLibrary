## WebViewLibrary

一句代码实现网页加载的webview工具类。

## WebViewLibrary 使用:

Step 1.先在 build.gradle(Project:XXXX) 的 repositories 添加:
```javascript
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
  
  Step 2. 然后在 build.gradle(Module:app) 的 dependencies 添加:
  ```javascript
  dependencies {
	        implementation 'com.github.ljw124:WebViewLibrary:1.0.4'
	}
	
```

Step 3. 在需要加载网页的地方开始使用:
 ```javascript
 /**
   * 参数1: 上下文;
   * 参数2: 需要加载网页的url;
   * 参数3: 跳转时的title。
   */
 WebViewActivity.loadUrl(MainActivity.this, "https://github.com/ljw124/WebViewLibrary.git", "WebViewLibrary");
```
