# zein-hijri
extended hijri date library from [nazir/go2hi](https://packagist.org/packages/nazir/go2hi) with [nesbot/carbon](https://packagist.org/packages/nesbot/carbon) syntax style

# Example
```PHP
<?php
require __DIR__ . '/vendor/autoload.php';

use Zein\Hijri\Hijri;

echo Hijri::now(); // get current date in hijri
// output : 09 Dzul Qa'dah 1443

echo Hijri::yesterday(); // yesterday
// output : 08 Dzul Qa'dah 1443

echo Hijri::yesterday(); // tomorrow
// output : 10 Dzul Qa'dah 1443

echo Hijri::now()->format('Y-m-d'); // tomorrow
// output : 1443-11-09

echo Hijri::get(15)->day()->ago(); // get 15 day ago
echo Hijri::get(1)->month()->ago(); // get 1 month ago
echo Hijri::get(2)->year()->ago(); // get 2 year ago
?>
```
