# CommandUnregister

Sunucunuzdaki istenmeyen komutları sunucudan siler.

### Nasıl Komut Eklerim?

Sunucunuzun dosyalarından plugin_data klasörüne girin. Ardından CommandUnregsiter klasörüne basın. Karşınıza commands.yml çıkacaktır. O dosyanın içinden silenecek komutları ayarlayabilirsiniz.

### Düzenleme
```yaml
Commands:
 - "commandName"
```

### Başka Bir Eklentiden Nasıl Kullanabilirim?

Evet, yanlış görmedin. Bu eklentiyi başka bir eklentiden yönetebilirsin. Kullanım:

use;
```php
use KurSkyTR\UnregisterCommand;
```
kullanım;
komut ekleme:
```php
UnregisterCommand::addUnregisterCommandList("commandName");
```
komut silme:
```php
UnregisterCommand::removeUnregisterCommandList("commandName");
```

Bu işlemler yapıldıktan sonra sunucuyu yeniden başlatmanız gerekmektedir.



