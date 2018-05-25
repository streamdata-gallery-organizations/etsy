---
name: Etsy
x-slug: etsy
description: Find handmade, vintage, and unique goods that express who you are.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
x-kinRank: "9"
x-alexaRank: "187"
tags: Etsy
created: "2018-05-25"
modified: "2018-05-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/apis.md
specificationVersion: "0.14"
apis:
- name: Etsy Get Countries Country
  x-api-slug: etsy
  description: Retrieves a Country by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//countries/{country_id}
  tags: Countries,Country
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/countriescountry-id-get-openapi.md
- name: Etsy Get Countries
  x-api-slug: etsy
  description: Finds all Country.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//countries
  tags: Countries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/countries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/countries-get-openapi.md
- name: Etsy Get Users User Favorites Listings
  x-api-slug: etsy
  description: Finds all favorite listings for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/favorites/listings
  tags: Users,Favorites,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfavoriteslistings-get-openapi.md
- name: Etsy Get Users User Favorites Listings Listing
  x-api-slug: etsy
  description: Finds a favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/favorites/listings/{listing_id}
  tags: Users,Favorites,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfavoriteslistingslisting-id-get-openapi.md
- name: Etsy Post Users User Favorites Listings Listing
  x-api-slug: etsy
  description: Creates a new favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/favorites/listings/{listing_id}
  tags: Users,Favorites,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfavoriteslistingslisting-id-post-openapi.md
- name: Etsy Delete Users User Favorites Listings Listing
  x-api-slug: etsy
  description: Delete a favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/favorites/listings/{listing_id}
  tags: Users,Favorites,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfavoriteslistingslisting-id-delete-openapi.md
- name: Etsy Get Users User Favorites Users
  x-api-slug: etsy
  description: Finds all favorite users for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/favorites/users
  tags: Users,Favorites,Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfavoritesusers-get-openapi.md
- name: Etsy Get Users User Favorites Users Target User
  x-api-slug: etsy
  description: Finds a favorite user for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/favorites/users/{target_user_id}
  tags: Users,Favorites,Users,Target,User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfavoritesuserstarget-user-id-get-openapi.md
- name: Etsy Post Users User Favorites Users Target User
  x-api-slug: etsy
  description: Creates a new favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/favorites/users/{target_user_id}
  tags: Users,Favorites,Users,Target,User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfavoritesuserstarget-user-id-post-openapi.md
- name: Etsy Delete Users User Favorites Users Target User
  x-api-slug: etsy
  description: Delete a favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/favorites/users/{target_user_id}
  tags: Users,Favorites,Users,Target,User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfavoritesuserstarget-user-id-delete-openapi.md
- name: Etsy Get Homepages Pickers
  x-api-slug: etsy
  description: Finds all FeaturedListingPicker in scope active.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//homepages/pickers/
  tags: Home Pages,Pickers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/homepagespickers-get-openapi.md
- name: Etsy Get Homepages Pickers Featured Listing Picker
  x-api-slug: etsy
  description: Retrieves a FeaturedListingPicker by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//homepages/pickers/{featured_listing_picker_id}
  tags: Home Pages,Pickers,Featured,Listing,Picker
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/homepagespickersfeatured-listing-picker-id-get-openapi.md
- name: Etsy Get Homepages Pickers Featured Listing Picker Featured
  x-api-slug: etsy
  description: Retrieves a set of FeaturedListing objects associated to a FeaturedListingPicker.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//homepages/pickers/{featured_listing_picker_id}/featured
  tags: Home Pages,Pickers,Featured,Listing,Picker,Featured
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/homepagespickersfeatured-listing-picker-idfeatured-get-openapi.md
- name: Etsy Get Homepages Pickers Featured Listing Picker Listings
  x-api-slug: etsy
  description: Retrieves a set of Listing objects associated to a FeaturedListingPicker.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//homepages/pickers/{featured_listing_picker_id}/listings
  tags: Home Pages,Pickers,Featured,Listing,Picker,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/homepagespickersfeatured-listing-picker-idlistings-get-openapi.md
- name: Etsy Get Homepages Pickers Featured Listing Picker Listings Active
  x-api-slug: etsy
  description: Retrieves a set of Listing objects associated to a FeaturedListingPicker
    in scope active.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//homepages/pickers/{featured_listing_picker_id}/listings/active
  tags: Home Pages,Pickers,Featured,Listing,Picker,Listings,Active
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/homepagespickersfeatured-listing-picker-idlistingsactive-get-openapi.md
- name: Etsy Get Homepages Listings
  x-api-slug: etsy
  description: Finds all FeaturedListings regardless of Listing state
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//homepages/listings/
  tags: Home Pages,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/homepageslistings-get-openapi.md
- name: Etsy Get Homepages Listings Active
  x-api-slug: etsy
  description: Finds all FeaturedListings that point to active Listings
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//homepages/listings/active
  tags: Home Pages,Listings,Active
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/homepageslistingsactive-get-openapi.md
- name: Etsy Get Homepages Listings Featured Listing
  x-api-slug: etsy
  description: Retrieves a FeaturedListing by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//homepages/listings/{featured_listing_id}
  tags: Home Pages,Listings,Featured,Listing
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/homepageslistingsfeatured-listing-id-get-openapi.md
- name: Etsy Get Homepages Listings Featured Listing Picker
  x-api-slug: etsy
  description: Retrieves a set of FeaturedListingPicker objects associated to a FeaturedListing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//homepages/listings/{featured_listing_id}/picker
  tags: Home Pages,Listings,Featured,Listing,Picker
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/homepageslistingsfeatured-listing-idpicker-get-openapi.md
- name: Etsy Get Homepages Listings Featured Listing Listing
  x-api-slug: etsy
  description: Retrieves a set of Listing objects associated to a FeaturedListing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//homepages/listings/{featured_listing_id}/listing
  tags: Home Pages,Listings,Featured,Listing,Listing
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/homepageslistingsfeatured-listing-idlisting-get-openapi.md
- name: Etsy Get Listings Listing Images Listing Image
  x-api-slug: etsy
  description: Retrieves a ListingImage by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings/{listing_id}/images/{listing_image_id}
  tags: Listings,Images,Listing,Image
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-idimageslisting-image-id-get-openapi.md
- name: Etsy Delete Listings Listing Images Listing Image
  x-api-slug: etsy
  description: Deletes a listing image
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings/{listing_id}/images/{listing_image_id}
  tags: Listings,Images,Listing,Image
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-idimageslisting-image-id-delete-openapi.md
- name: Etsy Post Listings Listing Images
  x-api-slug: etsy
  description: Upload a new listing image
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings/{listing_id}/images
  tags: Listings,Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-idimages-post-openapi.md
- name: Etsy Get Listings Listing Images
  x-api-slug: etsy
  description: Retrieves a set of ListingImage objects associated to a Listing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings/{listing_id}/images
  tags: Listings,Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-idimages-get-openapi.md
- name: Etsy Get Listings Listing
  x-api-slug: etsy
  description: Retrieves a Listing by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings/{listing_id}
  tags: Listings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-id-get-openapi.md
- name: Etsy Put Listings Listing
  x-api-slug: etsy
  description: Updates a Listing
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings/{listing_id}
  tags: Listings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-id-put-openapi.md
- name: Etsy Delete Listings Listing
  x-api-slug: etsy
  description: Deletes a Listing
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings/{listing_id}
  tags: Listings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-id-delete-openapi.md
- name: Etsy Get Listings Listing Favored By
  x-api-slug: etsy
  description: Retrieves a set of FavoriteListing objects associated to a Listing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings/{listing_id}/favored-by
  tags: Listings,Favored-by
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-idfavoredby-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-idfavoredby-get-openapi.md
- name: Etsy Get Listings Listing Shipping Info
  x-api-slug: etsy
  description: Retrieves a set of ShippingInfo objects associated to a Listing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings/{listing_id}/shipping/info
  tags: Listings,Shipping,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-idshippinginfo-get-openapi.md
- name: Etsy Post Listings Listing Shipping Info
  x-api-slug: etsy
  description: Creates a new ShippingInfo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings/{listing_id}/shipping/info
  tags: Listings,Shipping,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-idshippinginfo-post-openapi.md
- name: Etsy Get Listings Listing Payments
  x-api-slug: etsy
  description: Retrieves a set of ListingPayment objects associated to a Listing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings/{listing_id}/payments
  tags: Listings,Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingslisting-idpayments-get-openapi.md
- name: Etsy Get Listings Active
  x-api-slug: etsy
  description: Finds all active Listing
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings/active
  tags: Listings,Active
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingsactive-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listingsactive-get-openapi.md
- name: Etsy Get Shops Shop Listings Active
  x-api-slug: etsy
  description: Finds all active Listings associated with a Shop
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}/listings/active
  tags: Shops,Shop,Listings,Active
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idlistingsactive-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idlistingsactive-get-openapi.md
- name: Etsy Post Listings
  x-api-slug: etsy
  description: Creates a new Listing
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//listings
  tags: Listings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listings-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/listings-post-openapi.md
- name: Etsy Get Orders Order
  x-api-slug: etsy
  description: Retrieves a Order by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//orders/{order_id}
  tags: Orders,Order
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/ordersorder-id-get-openapi.md
- name: Etsy Get Orders Order Receipts
  x-api-slug: etsy
  description: Retrieves a set of Receipt objects associated to a Order.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//orders/{order_id}/receipts
  tags: Orders,Order,Receipts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/ordersorder-idreceipts-get-openapi.md
- name: Etsy Get Receipts Receipt
  x-api-slug: etsy
  description: Retrieves a Receipt by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//receipts/{receipt_id}
  tags: Receipts,Receipt
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/receiptsreceipt-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/receiptsreceipt-id-get-openapi.md
- name: Etsy Put Receipts Receipt
  x-api-slug: etsy
  description: Updates a Receipt
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//receipts/{receipt_id}
  tags: Receipts,Receipt
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/receiptsreceipt-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/receiptsreceipt-id-put-openapi.md
- name: Etsy Get Receipts Receipt Transactions
  x-api-slug: etsy
  description: Retrieves a set of Transaction objects associated to a Receipt.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//receipts/{receipt_id}/transactions
  tags: Receipts,Receipt,Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/receiptsreceipt-idtransactions-get-openapi.md
- name: Etsy Get Users User Recommended Listings
  x-api-slug: etsy
  description: Get recommended listings for an authenticated member. The number of
    listings returned may not match the specified limit if there is no activity from
    recommended shops.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/recommended_listings
  tags: Users,Recommended,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idrecommended-listings-get-openapi.md
- name: Etsy Post Users User Recommended Listings Rejects Listing S
  x-api-slug: etsy
  description: Registers rejections of recommended listings. Affects future recommended
    listings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/recommended_listings/rejects/{listing_ids}
  tags: Users,Recommended,Listings,Rejects,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idrecommended-listingsrejectslisting-ids-post-openapi.md
- name: Etsy Post Users User Recommended Listings Views Listing S
  x-api-slug: etsy
  description: Register viewings of recommended listings. Affects future recommended
    listings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/recommended_listings/views/{listing_ids}
  tags: Users,Recommended,Listings,Views,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idrecommended-listingsviewslisting-ids-post-openapi.md
- name: Etsy Get Regions Region
  x-api-slug: etsy
  description: Retrieves a Region by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//regions/{region_id}
  tags: Regions,Region
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/regionsregion-id-get-openapi.md
- name: Etsy Get Regions
  x-api-slug: etsy
  description: Finds all Region.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//regions
  tags: Regions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/regions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/regions-get-openapi.md
- name: Etsy Get Shipping Info Shipping Info
  x-api-slug: etsy
  description: Retrieves a ShippingInfo by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shipping/info/{shipping_info_id}
  tags: Shipping,Info,Shipping,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shippinginfoshipping-info-id-get-openapi.md
- name: Etsy Put Shipping Info Shipping Info
  x-api-slug: etsy
  description: Updates a ShippingInfo with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shipping/info/{shipping_info_id}
  tags: Shipping,Info,Shipping,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shippinginfoshipping-info-id-put-openapi.md
- name: Etsy Delete Shipping Info Shipping Info
  x-api-slug: etsy
  description: Deletes the ShippingInfo with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shipping/info/{shipping_info_id}
  tags: Shipping,Info,Shipping,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shippinginfoshipping-info-id-delete-openapi.md
- name: Etsy Get Shipping Templates Entries Shipping Template Entry
  x-api-slug: etsy
  description: Retrieves a ShippingTemplateEntry by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shipping/templates/entries/{shipping_template_entry_id}
  tags: Shipping,Templates,Entries,Shipping,Template,Entry
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shippingtemplatesentriesshipping-template-entry-id-get-openapi.md
- name: Etsy Put Shipping Templates Entries Shipping Template Entry
  x-api-slug: etsy
  description: Updates a ShippingTemplateEntry
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shipping/templates/entries/{shipping_template_entry_id}
  tags: Shipping,Templates,Entries,Shipping,Template,Entry
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shippingtemplatesentriesshipping-template-entry-id-put-openapi.md
- name: Etsy Delete Shipping Templates Entries Shipping Template Entry
  x-api-slug: etsy
  description: Deletes a ShippingTemplateEntry
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shipping/templates/entries/{shipping_template_entry_id}
  tags: Shipping,Templates,Entries,Shipping,Template,Entry
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shippingtemplatesentriesshipping-template-entry-id-delete-openapi.md
- name: Etsy Post Shipping Templates Entries
  x-api-slug: etsy
  description: Creates a new ShippingTemplateEntry
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shipping/templates/entries
  tags: Shipping,Templates,Entries
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shippingtemplatesentries-post-openapi.md
- name: Etsy Get Shipping Templates Shipping Template
  x-api-slug: etsy
  description: Retrieves a ShippingTemplate by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shipping/templates/{shipping_template_id}
  tags: Shipping,Templates,Shipping,Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shippingtemplatesshipping-template-id-get-openapi.md
- name: Etsy Delete Shipping Templates Shipping Template
  x-api-slug: etsy
  description: Deletes the ShippingTemplate with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shipping/templates/{shipping_template_id}
  tags: Shipping,Templates,Shipping,Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shippingtemplatesshipping-template-id-delete-openapi.md
- name: Etsy Put Shipping Templates Shipping Template
  x-api-slug: etsy
  description: Updates a ShippingTemplate
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shipping/templates/{shipping_template_id}
  tags: Shipping,Templates,Shipping,Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shippingtemplatesshipping-template-id-put-openapi.md
- name: Etsy Get Shipping Templates Shipping Template Entries
  x-api-slug: etsy
  description: Retrieves a set of ShippingTemplateEntry objects associated to a ShippingTemplate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shipping/templates/{shipping_template_id}/entries
  tags: Shipping,Templates,Shipping,Template,Entries
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shippingtemplatesshipping-template-identries-get-openapi.md
- name: Etsy Post Shipping Templates
  x-api-slug: etsy
  description: Creates a new ShippingTemplate
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shipping/templates
  tags: Shipping,Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shippingtemplates-post-openapi.md
- name: Etsy Get Shops Shop
  x-api-slug: etsy
  description: Retrieves a Shop by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}
  tags: Shops,Shop
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-id-get-openapi.md
- name: Etsy Put Shops Shop
  x-api-slug: etsy
  description: Updates a Shop
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}
  tags: Shops,Shop
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-id-put-openapi.md
- name: Etsy Get Shops Shop Receipts
  x-api-slug: etsy
  description: Retrieves a set of Receipt objects associated to a Shop.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}/receipts
  tags: Shops,Shop,Receipts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idreceipts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idreceipts-get-openapi.md
- name: Etsy Get Shops Shop Transactions
  x-api-slug: etsy
  description: Retrieves a set of Transaction objects associated to a Shop.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}/transactions
  tags: Shops,Shop,Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idtransactions-get-openapi.md
- name: Etsy Get Shops Shop Sections
  x-api-slug: etsy
  description: Retrieves a set of ShopSection objects associated to a Shop.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}/sections
  tags: Shops,Shop,Sections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idsections-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idsections-get-openapi.md
- name: Etsy Get Shops
  x-api-slug: etsy
  description: Finds all Shops. If there is a keywords parameter, finds shops with
    shop_name starting with keywords.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops
  tags: Shops
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shops-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shops-get-openapi.md
- name: Etsy Get Shops Shop Listings Featured
  x-api-slug: etsy
  description: Retrieves Listings associated to a Shop that are featured
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}/listings/featured
  tags: Shops,Shop,Listings,Featured
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idlistingsfeatured-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idlistingsfeatured-get-openapi.md
- name: Etsy Get Shops Shop Listings Inactive
  x-api-slug: etsy
  description: Retrieves Listings associated to a Shop that are inactive
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}/listings/inactive
  tags: Shops,Shop,Listings,Inactive
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idlistingsinactive-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idlistingsinactive-get-openapi.md
- name: Etsy Get Shops Shop Listings Expired
  x-api-slug: etsy
  description: Retrieves Listings associated to a Shop that are expired
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}/listings/expired
  tags: Shops,Shop,Listings,Expired
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idlistingsexpired-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idlistingsexpired-get-openapi.md
- name: Etsy Get Shops Shop Listings Inactive Listing
  x-api-slug: etsy
  description: Retrieves a Listing associated to a Shop that is inactive
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}/listings/inactive/{listing_id}
  tags: Shops,Shop,Listings,Inactive,Listing
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idlistingsinactivelisting-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idlistingsinactivelisting-id-get-openapi.md
- name: Etsy Get Shops Shop Listings Expired Listing
  x-api-slug: etsy
  description: Retrieves a Listing associated to a Shop that is inactive
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}/listings/expired/{listing_id}
  tags: Shops,Shop,Listings,Expired,Listing
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idlistingsexpiredlisting-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idlistingsexpiredlisting-id-get-openapi.md
- name: Etsy Post Shops Shop Appearance Banner
  x-api-slug: etsy
  description: Upload a new shop banner image
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}/appearance/banner
  tags: Shops,Shop,Appearance,Banner
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idappearancebanner-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idappearancebanner-post-openapi.md
- name: Etsy Delete Shops Shop Appearance Banner Shop Banner
  x-api-slug: etsy
  description: Deletes a shop banner image
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//shops/{shop_id}/appearance/banner/{shop_banner_id}
  tags: Shops,Shop,Appearance,Banner,Shop,Banner
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idappearancebannershop-banner-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/shopsshop-idappearancebannershop-banner-id-delete-openapi.md
- name: Etsy Get Sections Shop Section
  x-api-slug: etsy
  description: Retrieves a ShopSection by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//sections/{shop_section_id}
  tags: Sections,Shop,Section
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/sectionsshop-section-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/sectionsshop-section-id-get-openapi.md
- name: Etsy Put Sections Shop Section
  x-api-slug: etsy
  description: Updates a ShopSection with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//sections/{shop_section_id}
  tags: Sections,Shop,Section
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/sectionsshop-section-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/sectionsshop-section-id-put-openapi.md
- name: Etsy Delete Sections Shop Section
  x-api-slug: etsy
  description: Deletes the ShopSection with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//sections/{shop_section_id}
  tags: Sections,Shop,Section
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/sectionsshop-section-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/sectionsshop-section-id-delete-openapi.md
- name: Etsy Post Sections
  x-api-slug: etsy
  description: Creates a new ShopSection.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//sections
  tags: Sections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/sections-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/sections-post-openapi.md
- name: Etsy Get Categories Tag
  x-api-slug: etsy
  description: Retrieves a top-level Category by tag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//categories/{tag}
  tags: Categories,Tag
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/categoriestag-get-openapi.md
- name: Etsy Get Categories Tag Subtag
  x-api-slug: etsy
  description: Retrieves a second-level Category by tag and subtag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//categories/{tag}/{subtag}
  tags: Categories,Tag,Subtag
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/categoriestagsubtag-get-openapi.md
- name: Etsy Get Categories Tag Subtag Subsubtag
  x-api-slug: etsy
  description: Retrieves a third-level Category by tag, subtag and subsubtag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//categories/{tag}/{subtag}/{subsubtag}
  tags: Categories,Tag,Subtag,Subsubtag
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/categoriestagsubtagsubsubtag-get-openapi.md
- name: Etsy Get Taxonomy Categories
  x-api-slug: etsy
  description: Retrieves all top-level Categories.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//taxonomy/categories
  tags: Taxonomy,Categories
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/taxonomycategories-get-openapi.md
- name: Etsy Get Taxonomy Categories Tag
  x-api-slug: etsy
  description: Retrieves children of a top-level Category by tag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//taxonomy/categories/{tag}
  tags: Taxonomy,Categories,Tag
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/taxonomycategoriestag-get-openapi.md
- name: Etsy Get Taxonomy Categories Tag Subtag
  x-api-slug: etsy
  description: Retrieves children of a second-level Category by tag and subtag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//taxonomy/categories/{tag}/{subtag}
  tags: Taxonomy,Categories,Tag,Subtag
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/taxonomycategoriestagsubtag-get-openapi.md
- name: Etsy Get Taxonomy Tags
  x-api-slug: etsy
  description: Retrieves all related tags for the given tag set.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//taxonomy/tags
  tags: Taxonomy,Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/taxonomytags-get-openapi.md
- name: Etsy Get Taxonomy Tags Tags
  x-api-slug: etsy
  description: Retrieves all related tags for the given tag set.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//taxonomy/tags/{tags}
  tags: Taxonomy,Tags,Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/taxonomytagstags-get-openapi.md
- name: Etsy Get Transactions Transaction
  x-api-slug: etsy
  description: Retrieves a Transaction by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//transactions/{transaction_id}
  tags: Transactions,Transaction
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/transactionstransaction-id-get-openapi.md
- name: Etsy Get Treasuries Treasury
  x-api-slug: etsy
  description: Get a Treasury
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//treasuries/{treasury_id}
  tags: Treasuries
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/treasuriestreasury-id-get-openapi.md
- name: Etsy Get Treasuries
  x-api-slug: etsy
  description: Search Treasuries or else List all Treasuries
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//treasuries
  tags: Treasuries
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/treasuries-get-openapi.md
- name: Etsy Get Users User Treasuries
  x-api-slug: etsy
  description: Get a user's Treasuries
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/treasuries
  tags: Users,Treasuries
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idtreasuries-get-openapi.md
- name: Etsy Get Users User
  x-api-slug: etsy
  description: Retrieves a User by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-id-get-openapi.md
- name: Etsy Get Users User Shops
  x-api-slug: etsy
  description: Retrieves a set of Shop objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/shops
  tags: Users,Shops
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idshops-get-openapi.md
- name: Etsy Get Users User Favored By
  x-api-slug: etsy
  description: Retrieves a set of FavoriteUser objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/favored-by
  tags: Users,Favored-by
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfavoredby-get-openapi.md
- name: Etsy Get Users User Feedback As Subject
  x-api-slug: etsy
  description: Retrieves a set of Feedback objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/feedback/as-subject
  tags: Users,Feedback,As-subject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfeedbackassubject-get-openapi.md
- name: Etsy Get Users User Feedback As Author
  x-api-slug: etsy
  description: Retrieves a set of Feedback objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/feedback/as-author
  tags: Users,Feedback,As-author
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfeedbackasauthor-get-openapi.md
- name: Etsy Get Users User Feedback As Buyer
  x-api-slug: etsy
  description: Retrieves a set of Feedback objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/feedback/as-buyer
  tags: Users,Feedback,As-buyer
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfeedbackasbuyer-get-openapi.md
- name: Etsy Get Users User Feedback As Seller
  x-api-slug: etsy
  description: Retrieves a set of Feedback objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/feedback/as-seller
  tags: Users,Feedback,As-seller
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idfeedbackasseller-get-openapi.md
- name: Etsy Get Users User Orders
  x-api-slug: etsy
  description: Retrieves a set of Order objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/orders
  tags: Users,Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idorders-get-openapi.md
- name: Etsy Get Users User Receipts
  x-api-slug: etsy
  description: Retrieves a set of Receipt objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/receipts
  tags: Users,Receipts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idreceipts-get-openapi.md
- name: Etsy Get Users User Transactions
  x-api-slug: etsy
  description: Retrieves a set of Transaction objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/transactions
  tags: Users,Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idtransactions-get-openapi.md
- name: Etsy Get Users User Charges
  x-api-slug: etsy
  description: Retrieves a set of BillCharge objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/charges
  tags: Users,Charges
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idcharges-get-openapi.md
- name: Etsy Get Users User Payments
  x-api-slug: etsy
  description: Retrieves a set of BillPayment objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/payments
  tags: Users,Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idpayments-get-openapi.md
- name: Etsy Get Users User Shipping Templates
  x-api-slug: etsy
  description: Retrieves a set of ShippingTemplate objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/shipping/templates
  tags: Users,Shipping,Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idshippingtemplates-get-openapi.md
- name: Etsy Get Users User Payments Templates
  x-api-slug: etsy
  description: Retrieves a set of PaymentTemplate objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/payments/templates
  tags: Users,Payments,Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idpaymentstemplates-get-openapi.md
- name: Etsy Get Users User Addresses
  x-api-slug: etsy
  description: Retrieves a set of UserAddress objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/addresses
  tags: Users,Addresses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idaddresses-get-openapi.md
- name: Etsy Post Users User Addresses
  x-api-slug: etsy
  description: Creates a new UserAddress.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/addresses
  tags: Users,Addresses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idaddresses-post-openapi.md
- name: Etsy Get Payments Templates Payment Template
  x-api-slug: etsy
  description: Retrieves a PaymentTemplate by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//payments/templates/{payment_template_id}
  tags: Payments,Templates,Payment,Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/paymentstemplatespayment-template-id-get-openapi.md
- name: Etsy Put Payments Templates Payment Template
  x-api-slug: etsy
  description: Updates a PaymentTemplate
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//payments/templates/{payment_template_id}
  tags: Payments,Templates,Payment,Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/paymentstemplatespayment-template-id-put-openapi.md
- name: Etsy Post Payments Templates
  x-api-slug: etsy
  description: Creates a new PaymentTemplate
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//payments/templates
  tags: Payments,Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/paymentstemplates-post-openapi.md
- name: Etsy Get Payments Listing Payment
  x-api-slug: etsy
  description: Retrieves a ListingPayment by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//payments/{listing_payment_id}
  tags: Payments,Listing,Payment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/paymentslisting-payment-id-get-openapi.md
- name: Etsy Post Users User Avatar
  x-api-slug: etsy
  description: Upload a new user avatar image
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/avatar
  tags: Users,Avatar
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idavatar-post-openapi.md
- name: Etsy Get Users User Avatar Src
  x-api-slug: etsy
  description: Get avatar image source
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/avatar/src
  tags: Users,Avatar,Src
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idavatarsrc-get-openapi.md
- name: Etsy Get Users User Addresses User Address
  x-api-slug: etsy
  description: Retrieves a UserAddress by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/addresses/{user_address_id}
  tags: Users,Addresses,User,Address
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idaddressesuser-address-id-get-openapi.md
- name: Etsy Put Users User Addresses User Address
  x-api-slug: etsy
  description: Updates a UserAddress with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/addresses/{user_address_id}
  tags: Users,Addresses,User,Address
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idaddressesuser-address-id-put-openapi.md
- name: Etsy Delete Users User Addresses User Address
  x-api-slug: etsy
  description: Deletes the UserAddress with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//users/{user_id}/addresses/{user_address_id}
  tags: Users,Addresses,User,Address
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/usersuser-idaddressesuser-address-id-delete-openapi.md
- name: Etsy Get Featured Users
  x-api-slug: etsy
  description: Finds all FeaturedUser.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//featured/users
  tags: Featured,Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/featuredusers-get-openapi.md
- name: Etsy Get Featured Users Featured User
  x-api-slug: etsy
  description: Retrieves a FeaturedUser by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//featured/users/{featured_user_id}
  tags: Featured,Users,Featured,User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/featuredusersfeatured-user-id-get-openapi.md
- name: Etsy Get
  x-api-slug: etsy
  description: Get a list of all methods available.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//
  tags: ""
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/get-openapi.md
- name: Etsy Get Server Epoch
  x-api-slug: etsy
  description: Get server time, in epoch seconds notation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//server/epoch
  tags: Server,Epoch
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/serverepoch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/serverepoch-get-openapi.md
- name: Etsy Get Server Ping
  x-api-slug: etsy
  description: Check that the server is alive.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//server/ping
  tags: Server,Ping
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/serverping-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/serverping-get-openapi.md
- name: Etsy
  x-api-slug: etsy
  description: Etsy is a handmade marketplace. The Etsy API lets developers tap into
    the Etsy community, building their own Etsy-powered applications for the web,
    desktop and mobile devices. Applications built on the API will connect buyers
    with sellers, promote the handmade lifestyle, and support the craftspeople who
    sell on Etsy.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private
  tags: Etsy
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/etsy/master/_listings/etsy/openapi.md
x-common:
- type: x-api-json--authoritative
  url: http://apis.io/apisdef/etsy.json
- type: x-application-gallery
  url: https://www.etsy.com/apps/
- type: x-base
  url: https://openapi.etsy.com/
- type: x-blog
  url: http://www.etsy.com/blog/en/
- type: x-blog-rss
  url: https://blog.etsy.com/en/feed/
- type: x-copyright
  url: https://www.etsy.com/help/article/482/?ref=ftr
- type: x-crunchbase
  url: https://crunchbase.com/organization/etsy
- type: x-crunchbase
  url: http://www.crunchbase.com/company/etsy
- type: x-developer
  url: https://www.etsy.com/developers/
- type: x-email
  url: enaffiliates@etsy.com
- type: x-email
  url: selleraffiliate@etsy.com
- type: x-email
  url: developer@etsy.com
- type: x-email
  url: legal@etsy.com
- type: x-email
  url: dpo@etsy.com
- type: x-email
  url: dispute-resolution@etsy.com
- type: x-forum
  url: https://www.etsy.com/developers/discussion
- type: x-github
  url: https://github.com/etsy
- type: x-privacy
  url: https://www.etsy.com/help/article/480/?ref=ftr
- type: x-terms-of-service
  url: https://www.etsy.com/help/article/479/?ref=ftr
- type: x-transparency-report
  url: http://blog.etsy.com/news/files/2015/07/Etsy_TransparencyReport_2014.pdf
- type: x-twitter
  url: https://twitter.com/Etsy
- type: x-website
  url: http://www.etsy.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---