# DevHenry

_Light Weight Library Used to Automate SQL Query has SQLite Support too_

## Usage

#### Creating A Table

```php
<?php

use DevHenry\Model;

$model = new Model("users", [
    Model::INT("id", true),
    Model::TEXT("email"),
    Model::TEXT("firstname"),
    Model::TEXT("lastname"),
    Model::TEXT("password"),
    Model::TEXT("balance"),
]);

/**
 * This Will Create The Table and Save the Query in '/generated' folder in the same folder where this file is located
 */
Loader::load($model);

```
