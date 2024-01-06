# silverstripe-empty-extension

Sometimes third-party modules will apply extensions by default, which you would rather they didn't.

However there isn't a straight-forward mechanism to un-apply the extensions or to remove/replace the config.yml block that is applying them.

This is a super simple module, which contains an empty extension, which can then be used in inconjunction with the Injector to simply replace the extension you don't want.

Requires Silverstripe 4 or 5+.

For example:

```yml
SilverStripe\Core\Injector\Injector:
  Namespace\ExtensionClassToBeReplaced:
    class: Fromholdio\EmptyExtension\EmptyExtension
```
