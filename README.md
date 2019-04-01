# Social Share Links 2019
List of commonly used social media share deep links and URL schema (2019)
***Tested on 01 April 2019**

### Whatsapp

------------
#### Browser Supports
|  Browsers | Supports  |
| ------------ | ------------ |
|  Chrome (iOS) | Yes  |
| Safari (iOS)  | Yes  |
|Chrome (Android)|Yes|

#### Demo
```javascript
var linkElement = document.createElement('a');
linkElement.style.visibility = 'hidden';
linkElement.style.position = 'absolute';
linkElement.href = hrefStr;
document.body.appendChild('whatsapp://send?text=Hello World');
linkElement.click();
linkElement.remove();
```

### Line
------------
#### Browser Supports
|  Browsers | Supports  |
| ------------ | ------------ |
|  Chrome (iOS) | Yes  |
| Safari (iOS)  | Yes  |
|Chrome (Android)|Yes|

#### Demo
```javascript
window.open('https://lineit.line.me/share/ui?url=www.google.com&text=Hello World','_blank');
```

### WeChat
------------
Offical deep link is not supported by WeChat, below is unoffical, which does not support share with text. It simply open WeChat

#### Browser Supports
|  Browsers | Supports  |
| ------------ | ------------ |
|  Chrome (iOS) | Yes  |
| Safari (iOS)  | Yes  |
|Chrome (Android)|Yes|

#### Demo
```javascript
var linkElement = document.createElement('a');
linkElement.style.visibility = 'hidden';
linkElement.style.position = 'absolute';
linkElement.href = hrefStr;
document.body.appendChild('weixin://');
linkElement.click();
linkElement.remove();
```
### Email
------------
#### Browser Supports
|  Browsers | Supports  |
| ------------ | ------------ |
|  Chrome (iOS) | Yes  |
| Safari (iOS)  | Yes  |
|Chrome (Android)|Yes|
|IE11(Desktop)|Yes|
|Chrome(Desktop)|Yes|
|Firefox(Desktop)|Yes|

#### Demo
```javascript
var linkElement = document.createElement('a');
linkElement.style.visibility = 'hidden';
linkElement.style.position = 'absolute';
linkElement.href = hrefStr;
document.body.appendChild('mailto:?body=Hello World&subject=Subject');
linkElement.click();
linkElement.remove();
```
