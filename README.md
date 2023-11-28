## Laravel Helpers
This package provides the useful Laravel helper functions and allows you to use them in Laravel projects.

## Installation

Install the package with Composer: 

```
composer require surazdott/laravel-helpers
```

## Example
```
<?php

namespace App\Http\Controllers;

class HomeController extends Controller
{
    /**
     * Show the application dashboard.
     *
     * @return  \Illuminate\Contracts\Support\Renderable
     */
    public function index()
    {
        $data['timezones'] = timezones(); // array response
        $data['views'] = countViews(1000); // 1K views
        return view('home', $data);
    }
}

```

## Usage
#### # Get IP Address
```
/**
 * Get User Current IP Address
 *
 * @return $ip string
*/
function getIPAddress(): string
```
#### # Get Timezones
```
/**
 * Timezone lists
 *
 * @return array
*/
function timezones(): array
```
#### # Get Active Page
```
/**
 * Current active page
 *
 * @param $uri string
 * @return string
*/
function active($uri = ''): string
```
#### # Get file format
```
/**
 * Get File format
 *
 * @param $bytes string
 * @return string
*/
function active(): string
```
#### # Count Views
```
/**
 * Count Views
 *
 * @return string
*/
function countViews($views): string
```
#### # Protect Email address
```
/**
 * Hide email address partially
 *
 * @param $email string
 * @return $email string
*/
function protectEmail($email): string
```
## License
Laravel helpers is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT), this project is licensed under the same license.