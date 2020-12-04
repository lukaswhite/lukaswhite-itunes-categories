# iTunes Categories

This simple PHP package simply defines all of the valid categories for iTunes podcasts.

## Installation

```bash
composer require lukaswhite/itunes-categories
```

## Usage

```php
use Lukaswhite\ItunesCategories\Categories;

$categories = new Categories();

$categories->arr();
```

This simply returns a nested associative array of all the categories and their children.

You can check whether categories exist:

```php
$categories->has('Sports') // true
$categories->has('Sports', 'Football'); // true
```

