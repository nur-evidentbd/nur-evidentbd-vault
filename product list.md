

## Product properties



|   |   |   |
|---|---|---|
|Attribute|Type|Description|
|id|integer|Unique identifier for the resource. read-only|
|name|string|Product name.|
|slug|string|Product slug.|
|permalink|string|Product URL. read-only|
|date_created|date-time|The date the product was created, in the site's timezone. read-only|
|date_created_gmt|date-time|The date the product was created, as GMT. read-only|
|date_modified|date-time|The date the product was last modified, in the site's timezone. read-only|
|date_modified_gmt|date-time|The date the product was last modified, as GMT. read-only|
|type|string|Product type. Options: simple , grouped , external and variable . Default is simple .|
|status|string|Product status (post status). Options: draft , pending , private and publish . Default is publish .|
|featured|boolean|Featured product. Default is false .|
|catalog_visibility|string|Catalog visibility. Options: visible , catalog , search and hidden . Default is visible .|
|description|string|Product description.|
|short_description|string|Product short description.|
|sku|string|Unique identifier.|
|price|string|Current product price. read-only|
|regular_price|string|Product regular price.|
|sale_price|string|Product sale price.|
|date_on_sale_from|date-time|Start date of sale price, in the site's timezone.|
|date_on_sale_from_gmt|date-time|Start date of sale price, as GMT.|
|date_on_sale_to|date-time|End date of sale price, in the site's timezone.|
|date_on_sale_to_gmt|date-time|End date of sale price, as GMT.|
|price_html|string|Price formatted in HTML. read-only|
|on_sale|boolean|Shows if the product is on sale. read-only|
|purchasable|boolean|Shows if the product can be bought. read-only|
|total_sales|integer|Amount of sales. read-only|
|virtual|boolean|If the product is virtual. Default is false .|
|downloadable|boolean|If the product is downloadable. Default is false .|
|downloads|array|List of downloadable files. See Product - Downloads properties|
|download_limit|integer|Number of times downloadable files can be downloaded after purchase. Default is -1 .|
|download_expiry|integer|Number of days until access to downloadable files expires. Default is -1 .|
|external_url|string|Product external URL. Only for external products.|
|button_text|string|Product external button text. Only for external products.|
|tax_status|string|Tax status. Options: taxable , shipping and none . Default is taxable .|
|tax_class|string|Tax class.|
|manage_stock|boolean|Stock management at product level. Default is false .|
|stock_quantity|integer|Stock quantity.|
|stock_status|string|Controls the stock status of the product. Options: instock , outofstock , onbackorder . Default is instock .|
|backorders|string|If managing stock, this controls if backorders are allowed. Options: no , notify and yes . Default is no .|
|backorders_allowed|boolean|Shows if backorders are allowed. read-only|
|backordered|boolean|Shows if the product is on backordered. read-only|
|sold_individually|boolean|Allow one item to be bought in a single order. Default is false .|
|weight|string|Product weight.|
|dimensions|object|Product dimensions. See Product - Dimensions properties|
|shipping_required|boolean|Shows if the product need to be shipped. read-only|
|shipping_taxable|boolean|Shows whether or not the product shipping is taxable. read-only|
|shipping_class|string|Shipping class slug.|
|shipping_class_id|integer|Shipping class ID. read-only|
|reviews_allowed|boolean|Allow reviews. Default is true .|
|average_rating|string|Reviews average rating. read-only|
|rating_count|integer|Amount of reviews that the product have. read-only|
|related_ids|array|List of related products IDs. read-only|
|upsell_ids|array|List of up-sell products IDs.|
|cross_sell_ids|array|List of cross-sell products IDs.|
|parent_id|integer|Product parent ID.|
|purchase_note|string|Optional note to send the customer after purchase.|
|categories|array|List of categories. See Product - Categories properties|
|tags|array|List of tags. See Product - Tags properties|
|images|array|List of images. See Product - Images properties|
|attributes|array|List of attributes. See Product - Attributes properties|
|default_attributes|array|Defaults variation attributes. See Product - Default attributes properties|
|variations|array|List of variations IDs. read-only|
|meta_data|array|Meta data. See Product - Meta data properties|


