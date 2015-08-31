Filter
======

The Filter component provides a API for data filtering.

### What is a filter?

In the physical world, a filter is typically used for removing unwanted portions of input, and the desired portion of the input passes through as filter output (e.g., coffee). In such scenarios, a filter is an operator that produces a subset of the input. This type of filtering is useful for web applications - removing illegal input, trimming unnecessary white space, etc.

## Basic usage of filters

Having this filter definition established provides the foundation for Owl\Filter\FilterInterface, which requires a single method named filter() to be implemented by a filter class.

Following is a basic example of using

```php
$trimFilter = new \Owl\Filter\Trim();

var_dump($trimFilter->filter(' string ')); // string(6) "string"
```

## How to write own filter

An example how to do it:

```php
namespace App\Filter;

class MyOwnTrim extends \Owl\Filter\AbstractFilter
{
    public fn filter(var value) -> var
    {
		return trim(value);
    }
}
```
