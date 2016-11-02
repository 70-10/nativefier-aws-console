# nativefier-aws-console

## Usage

### Settings username and password

**`inject.js`**

```js
(window.onload = function() {
  setTimeout(function () {
    document.getElementById("username").value="<YOUR USER NAME>";
    document.getElementById("password").value="<YOUR PASSWORD>";
    document.getElementById("signin_form").submit();
  }, 1000);
})();
```

### Build

```sh
$ nativefier --name "AWS Console" --icon ./aws.icns --inject ./inject.js https://<AWS-account-ID-or-alias>.signin.aws.amazon.com/console
```
