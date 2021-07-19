# Contributing

## Getting Started
Make sure you fork the repository so you can modify it locally, this will help with confliction in the future.

## Playercards
1. Dimensions should be no greater than **275x84**.
2. Should contain a transparent and non-transparent variant.
3. Should be saved as a **PNG** and pushed through a **lossless compression**. (We recommend Squoosh)

## Banners
1. All banners dimensions should be no greater than **1900x400**.
2. Should be saved as a **JPG** and pushed through a **lossless compression**. (We recommend Squoosh)

## Naming
All **banners** should be prefixed by `banner_` in the file name.
All **playercards** should be prefixed with a `_transparent` if it is the transparent varient.

## Modifying JSON
Please make sure all modifications to JSON are validated through some sort of JSON lint/validation tool such as [JSON Lint](https://jsonlint.com/). When modifying the JSON, you always want to add your new item to the end of the file. 

### Object Example
```js
{
    "id": 0,
    "name": "Default",
    "file": "dotted_generic",
    "level": 0,
    "price": 0,
    "secret": false,
    "order": 1
  }
```
1. Make sure the `name` is unique and cannot be accidentally reused by other submissions in the future
2. Make sure the `file` field is the same name as the image (if it is a playercard, do not add the `_transparent` part)
3. Do **not** modify the `order`, `level`, `price` or `secret` field unless you are an authorized contributor by Keyma.sh.

## Submitting
All submissions should be done as a **Pull Request** from your forked repository. It will go through a submission process and once approved will be added into the game within 2-4 weeks. Main reason for the delay is that we have to evaluate the worth of each item and experience level needed, we also don't plan major updates and since this data is stored server-side we don't typically push updates constantly for the server side of Keyma.sh