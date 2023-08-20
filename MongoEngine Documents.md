
## Product

```python
import mongoengine as db

class Product(db.Document):
    id = db.IntField(unique=True)
    name = db.StringField(required=True)
    slug = db.StringField()
    permalink = db.StringField()
    date_created = db.DateTimeField()
    date_created_gmt = db.DateTimeField()
    date_modified = db.DateTimeField()
    date_modified_gmt = db.DateTimeField()
    type = db.StringField(default="simple", choices=["simple", "grouped", "external", "variable"])
    status = db.StringField(default="publish", choices=["draft", "pending", "private", "publish"])
    featured = db.BooleanField(default=False)
    catalog_visibility = db.StringField(default="visible", choices=["visible", "catalog", "search", "hidden"])
    description = db.StringField()
    short_description = db.StringField()
    sku = db.StringField(unique=True)
    price = db.StringField()
    regular_price = db.StringField()
    sale_price = db.StringField()
    date_on_sale_from = db.DateTimeField()
    date_on_sale_from_gmt = db.DateTimeField()
    date_on_sale_to = db.DateTimeField()
    date_on_sale_to_gmt = db.DateTimeField()
    price_html = db.StringField(read_only=True)
    on_sale = db.BooleanField()
    purchasable = db.BooleanField()
    total_sales = db.IntField()
    virtual = db.BooleanField(default=False)
    downloadable = db.BooleanField(default=False)
    downloads = db.ListField(db.DictField())  # Define the structure for downloadable files
    download_limit = db.IntField(default=-1)
    download_expiry = db.IntField(default=-1)
    external_url = db.StringField()
    button_text = db.StringField()
    tax_status = db.StringField(default="taxable", choices=["taxable", "shipping", "none"])
    tax_class = db.StringField()
    manage_stock = db.BooleanField(default=False)
    stock_quantity = db.IntField()
    stock_status = db.StringField(default="instock", choices=["instock", "outofstock", "onbackorder"])
    backorders = db.StringField(default="no", choices=["no", "notify", "yes"])
    backorders_allowed = db.BooleanField()
    backordered = db.BooleanField()
    sold_individually = db.BooleanField(default=False)
    weight = db.StringField()
    dimensions = db.DictField()  # Define the structure for product dimensions
    shipping_required = db.BooleanField()
    shipping_taxable = db.BooleanField(read_only=True)
    shipping_class = db.StringField()
    shipping_class_id = db.IntField(read_only=True)
    reviews_allowed = db.BooleanField(default=True)
    average_rating = db.StringField(read_only=True)
    rating_count = db.IntField(read_only=True)
    related_ids = db.ListField(db.IntField(read_only=True))
    upsell_ids = db.ListField(db.IntField())
    cross_sell_ids = db.ListField(db.IntField())
    parent_id = db.IntField()
    purchase_note = db.StringField()
    categories = db.ListField(db.DictField())  # Define the structure for product categories
    tags = db.ListField(db.DictField())  # Define the structure for product tags
    images = db.ListField(db.DictField())  # Define the structure for product images
    attributes = db.ListField(db.DictField())  # Define the structure for product attributes
    default_attributes = db.ListField(db.DictField())  # Define the structure for default variation attributes
    variations = db.ListField(db.IntField(read_only=True))
    meta_data = db.ListField(db.DictField())  # Define the structure for meta data

```