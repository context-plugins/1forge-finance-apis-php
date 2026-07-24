# Forex

```php
$forexController = $client->getForexController();
```

## Class Name

`ForexController`

## Methods

* [Get Quotes for All Symbols](../../doc/controllers/forex.md#get-quotes-for-all-symbols)
* [Get a List of Symbols for Which We Provide Real-Time Quotes](../../doc/controllers/forex.md#get-a-list-of-symbols-for-which-we-provide-real-time-quotes)


# Get Quotes for All Symbols

Get quotes

Find out more: [http://1forge.com/forex-data-api](http://1forge.com/forex-data-api)

```php
function getQuotesForAllSymbols(): void
```

## Response Type

**200**: A list of quotes

`void`

## Example Usage

```php
$forexController = $client->getForexController();

try {
    $forexController->getQuotesForAllSymbols();
} catch (ApiException $exp) {
    echo 'Caught:', $exp;
}
```


# Get a List of Symbols for Which We Provide Real-Time Quotes

Symbol List

Find out more: [http://1forge.com/forex-data-api](http://1forge.com/forex-data-api)

```php
function getAListOfSymbolsForWhichWeProvideRealTimeQuotes(): array
```

## Response Type

**200**: A list of symbols

`string[]`

## Example Usage

```php
$forexController = $client->getForexController();

try {
    $result = $forexController->getAListOfSymbolsForWhichWeProvideRealTimeQuotes();
    echo 'string[]:';
    var_dump($result);
} catch (ApiException $exp) {
    echo 'Caught:', $exp;
}
```

