Twig extension : array
=====================

## Installation & Requirements

Install with [Composer](https://getcomposer.org):

```shell script
composer require jmf/twig-array
```

## Usage in Twig templates

### array_set()

Sets a specific key in an array.

```html
{% set values = {} %}

{% set values = values|array_set('foo', 'bar') %}
```

### array_unset()

Unsets a specific key in an array.

```html
{% set values = {'foo': 'bar'} %}

{% set values = values|array_unset('foo') %}
```

### array_push()

Appends a new value at the end of an array.

```html
{% set values = {'foo'} %}

{% set values = values|array_push('bar') %}
```

### array_pop()

Removes the last item of an array.

```html
{% set values = {'foo', 'bar'} %}

{% set values = values|array_pop() %}
```

### array_unshift()

Appends a new value at the beginning of an array.

```html
{% set values = {'foo'} %}

{% set values = values|array_unshift('bar') %}
```

### array_shift()

Removes the first item of an array.

```html
{% set values = {'foo', 'bar'} %}

{% set values = values|array_shift() %}
```
