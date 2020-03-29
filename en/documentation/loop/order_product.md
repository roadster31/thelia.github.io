---
layout: loop
title: Order product Loop
description: Order product loop displays Order products information.
sidebar: loop
lang: en
subnav: loop_order_product
uses_global_argument: true
returns_global_outputs: { countable : true, timestampable : true, versionable : false }
type: order_product
arguments :
    - {name: "order", description: "A single order id.", example: "order=\"2\"", mandatory: "true"}
    - {name: "id", description: "A single or a list of order product ids.", example: "id=\"2\", id=\"1,4,7\""}
    - {name: "virtual", description: "A boolean value.", example: "new=\"yes\""}
outputs :
    - {name: "$ID", description: "the order product id"}
    - {name: "$REF", description: "the order product reference"}
    - {name: "$PRODUCT_SALE_ELEMENTS_REF", description: "the order product sale elements reference"}
    - {name: "$WAS_NEW", description: "whatever the order product sale elements was new or not"}
    - {name: "$WAS_IN_PROMO", description: "whatever the order product sale elements was in promo or not"}
    - {name: "$WEIGHT", description: "the order product sale elements weight"}
    - {name: "$TITLE", description: "the order product title"}
    - {name: "$CHAPO", description: "the order product short description"}
    - {name: "$DESCRIPTION", description: "the order product description"}
    - {name: "$POSTSCRIPTUM", description: "the order product postscriptum"}
    - {name: "$VIRTUAL", description: "whatever the order product is a virtual product or not"}
    - {name: "$VIRTUAL_DOCUMENT", description: "the name of the file if the product is virtual."}
    - {name: "$QUANTITY", description: "the order product ordered quantity"}
    - {name: "$PRICE", description: "the order product price (unit price)"}
    - {name: "$PRICE_TAX", description: "the order product taxes (unit price)"}
    - {name: "$TAXED_PRICE", description: "the order product price including taxes (unit price)"}
    - {name: "$PROMO_PRICE", description: "the order product in promo price (unit price)"}
    - {name: "$PROMO_PRICE_TAX", description: "the order product in promo price taxes (unit price)"}
    - {name: "$TAXED_PROMO_PRICE", description: "the order product in promo price including taxes (unit price)"}
    - {name: "$TOTAL_PRICE", description: "the order product price (total price)", from_version: "2.3"}
    - {name: "$TOTAL_TAXED_PRICE", description: "the order product price including taxes (total price)", from_version: "2.3"}
    - {name: "$TOTAL_PROMO_PRICE", description: "the order product in promo price (total price)", from_version: "2.3"}
    - {name: "$TOTAL_TAXED_PROMO_PRICE", description: "the order product in promo price including taxes (total price)", from_version: "2.3"}
    - {name: "$CART_ITEM_ID", description: "The related Cart Item ID of this order product", from_version: "2.4"}
    - {name: "$TAX_RULE_TITLE", description: "the tax rule title for this item"}
    - {name: "$TAX_RULE_DESCRIPTION", description: "the tax rule description for this item"}
    - {name: "$PARENT", description: "the parent product in the cart, if the current product has one"}
    - {name: "$EAN_CODE", description: "the product ean code"}
    - {name: "$REAL_PRICE", description: "the absolute item price excluding tax, either promo or normal, depending on IS_PROMO status", from_version: "2.4"}
    - {name: "$REAL_TAXED_PRICE", description: "the absolute item item price including tax, either promo or normal, depending on IS_PROMO status", from_version: "2.4"}
    - {name: "$REAL_TOTAL_PRICE", description: "the absolute total price excluding tax, either promo or normal, depending on IS_PROMO status", from_version: "2.4"}
    - {name: "$REAL_TOTAL_TAXED_PRICE", description: "the absolute total price including tax, either promo or normal, depending on IS_PROMO status", from_version: "2.4"}    
---
