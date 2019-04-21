# ESLint 规则开启/关闭

------

> /* eslint eqeqeq: 0, curly: 2 */

* "off" or 0: 关闭这条规则
* "warn" or 1: 开启规则，如果校验有问题则抛出警告
* "error" or 2: 开启规则，如果校验有问题则抛出错误

1、关闭/开启所有规则校验

```javascript
/* eslint-disable */

/* eslint-enable */
```

2、关闭/开启校验部分具体的规则校验

```javascript
/* eslint-disable no-alert, no-console */

/* eslint-enable no-alert, no-console */
```

3、关闭当前行的所有规则校验

```javascript
alert('foo'); // eslint-disable-line
```

4、关闭下一行的所有规则校验

```javascript
// eslint-disable-next-line
alert('foo');
```

5、关闭当前行的具体规则校验

```javascript
alert('foo'); // eslint-disable-line no-alert
```

6、关闭下一行的具体规则校验

```javascript
// eslint-disable-next-line no-alert
alert('foo');
```