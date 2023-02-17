Flashing with single message
```php
session()->flash('success', 'Invoice has been created!')
```
Flashing with multiple message
```php
session()->flash('success', [
      'Invoice has been created!',
      'And please make payment!',
])
```
## Flashing Types
- success
- warning
- info
- danger
