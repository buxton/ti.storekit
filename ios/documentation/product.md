# Ti.Storekit.Product

## Description

A _Ti.Storekit_ module object which represents a product from the in-app store.

## Properties

### Ti.Storekit.Product.title[string] (read-only)

The title of the product.

### Ti.Storekit.Product.description[string] (read-only)

The description of the product.

### Ti.Storekit.Product.price[double] (read-only)

The price of the product.

### Ti.Storekit.Product.formattedPrice[string] (read-only)

The price of the product, formatted for the store's locale.

### Ti.Storekit.Product.introductoryPrice[Discount] (read-only)

(iOS 11.2+)

The introductory price of the product, served as a `Discount` proxy.
Includes the following properties:
  * price (Number)
  * priceLocale (String)
  * subscriptionPeriod (Dictionary) { numberOfUnits (Number), unit (number) }
  * numberOfPeriods (Number)
  * paymentMode (Number, `DISCOUNT_PAYMENT_MODE_*`)

### Ti.Storekit.Product.subscriptionPeriod[Dictionary] (read-only)

(iOS 11.2+)

The subscription period of the product, served as a dictionary with the following properties.
  * numberOfUnits (Number)
  * unit (Number, `PERIOD_UNIT_*`)

### Ti.Storekit.Product.locale[string] (read-only)

The locale of the product.

### Ti.Storekit.Product.identifier[string] (read-only)

The product's identifier in the in-app store.

### Ti.Storekit.Product.downloadable[boolean] (read-only)

A boolean value that indicates whether the App Store has downloadable content for this product.

You can associate a set of data files with the iTunes Connect record you created for a product. The value of this property is true if at least one file has been associated with the product.

### Ti.Storekit.Product.downloadContentLengths[array<number>] (read-only)

The lengths of the downloadable files available for this product.

The array holds number objects, each of which holds value that is the size of one of the downloadable files (in bytes).

### Ti.Storekit.Product.downloadContentVersion[string] (read-only)

A string that identifies which version of the content is available for download.

The version string is formatted as a series of integers separated by periods.
