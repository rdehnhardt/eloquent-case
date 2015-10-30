# eloquent-case
Set attributes to upper or lower case automatically

## Installation

Run the following command to get the latest version package

```
composer require baconfy/eloquent-case
```

```php
// app/Customer.php
namespace App;

use Illuminate\Database\Eloquent\Model;
use Baconfy\EloquentCase\Traits\TransformUpperCase;

class Customer extends Model
{
    use TransformUpperCase;

    /**
     * The attributes that aren't upper case. (optional)
     *
     * @var array
     */
    protected $guardedCase = ['email', 'password'];
}
```

```php
// app/Customer.php
namespace App;

use Illuminate\Database\Eloquent\Model;
use Baconfy\EloquentCase\Traits\TransformUpperCase;

class Customer extends Model
{
    use TransformLowerCase;

    /**
     * The attributes that aren't lower case. (optional)
     *
     * @var array
     */
    protected $guardedCase = ['name'];
}
```

<a name="contributing"></a>
## Contributing

Contributions are welcomed; to keep things organized, all bugs and requests should be opened on github issues tab for the main project in the [baconfy/eloquent-case/issues](https://github.com/baconfy/eloquent-case/issues).

All pull requests should be made to the branch Develop, so they can be tested before being merged into the master branch.

<a name="faq"></a>
## Having problems?

If you are having problems with the use of this package, there is likely someone has faced the same problem. You can find common answers to their problems:

* [Github Issues](https://github.com/baconfy/eloquent-case/issues?page=1&state=closed)

<a name="license"></a>
### License

The eloquent-case package is open source software licensed under the [license MIT](http://opensource.org/licenses/MIT)

