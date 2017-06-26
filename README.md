Laravel Country Validation Rule
================================

A simple country validation rule for Laravel

## How to install

1. Clone or download this repo.
2. Copy the ``custom`` folder into your Laravel project's ``app/Validators`` directory.
3. Add the follwing to a service provider:

```
Validator::extend('country', \App\Validators\CountryValidator::class);
```

4. Add a validation error message in ``app/lang/en/validation.php`` in the validation language lines array:

```
"country" => "The :attribute must be a country",
```

## How to use

Simply use the ``country`` rule like any other validation rule.

```
$rules = [
    'country' => 'required|country'
];
```

Forked from [Sailr.co](http://sailr.co).

## License

####tl;dr: do whatever you want with it, but don't blame us if it breaks something.

This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <http://unlicense.org>