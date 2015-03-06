# BootstrapCake Shell Template

BootstrapCake is a shell template for rapidly developing beautiful Bootstrap themed CakePHP applications through the CakePHP console. The default template uses the ugly CakePHP styling but this template makes your app look beautiful by default.

## Requirements

* [CakePHP](http://cakephp.org/) >= 2.3
* [Bootstrap](http://getbootstrap.com/) >= 3.0

## Installation

In your current project folder you can clone BootstrapCake using:
```bash
git clone https://github.com/lucascampelo/BootstrapCake.git Plugin/BootstrapCake
```

OR

Using as Submodule:
```bash
git submodule add https://github.com/lucascampelo/BootstrapCake.git Plugin/BootstrapCake
```
PS: If you have problem using submodule, try `git submodule init` before add submodule, and `git submodule update` after.

OR

Extract the files into the proper directory (probably `app\Plugin`) and rename folder to `BootstrapCake`.

## Usage
Can you generate views and controllers to use in your project with commands below:
* Generating Controller:
```bash
Console\cake bake controller Users -t bootstrap
```

* Generating View:
```bash
Console\cake bake view Users -t bootstrap
```


## Customization
Can you use Bootstrap Layout and elements in your own Views and Controllers importing plugin files:
* On view files:
```php
# Views\Pages\bootstrap-example.ctp
echo echo $this->element('BootstrapCake.navigation');
```

* On controllers files:
```php
# Controller\UsersController.php
public function beforeFilter() {
    // your app code here
    $this->layout = 'BootstrapCake.bootstrap';
}
```

To customize views, I sugest you generate view files using `Console\cake bake` explained above and make your own changes.

Thanks for use!