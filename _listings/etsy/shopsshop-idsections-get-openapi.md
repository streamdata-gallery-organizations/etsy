---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Get Shops Shop Sections
  description: Retrieves a set of ShopSection objects associated to a Shop.
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /countries/{country_id}:
    get:
      summary: Get Countries Country
      description: Retrieves a Country by id.
      operationId: getCountriesCountry
      x-api-path-slug: countriescountry-id-get
      responses:
        200:
          description: OK
      tags:
      - Countries
      - Country
  /countries:
    get:
      summary: Get Countries
      description: Finds all Country.
      operationId: getCountries
      x-api-path-slug: countries-get
      responses:
        200:
          description: OK
      tags:
      - Countries
  /users/{user_id}/favorites/listings:
    get:
      summary: Get Users User Favorites Listings
      description: Finds all favorite listings for a user
      operationId: getUsersUserFavoritesListings
      x-api-path-slug: usersuser-idfavoriteslistings-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Listings
  /users/{user_id}/favorites/listings/{listing_id}:
    get:
      summary: Get Users User Favorites Listings Listing
      description: Finds a favorite listing for a user
      operationId: getUsersUserFavoritesListingsListing
      x-api-path-slug: usersuser-idfavoriteslistingslisting-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Listings
    post:
      summary: Post Users User Favorites Listings Listing
      description: Creates a new favorite listing for a user
      operationId: postUsersUserFavoritesListingsListing
      x-api-path-slug: usersuser-idfavoriteslistingslisting-id-post
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Listings
    delete:
      summary: Delete Users User Favorites Listings Listing
      description: Delete a favorite listing for a user
      operationId: deleteUsersUserFavoritesListingsListing
      x-api-path-slug: usersuser-idfavoriteslistingslisting-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Listings
  /users/{user_id}/favorites/users:
    get:
      summary: Get Users User Favorites Users
      description: Finds all favorite users for a user
      operationId: getUsersUserFavoritesUsers
      x-api-path-slug: usersuser-idfavoritesusers-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Users
  /users/{user_id}/favorites/users/{target_user_id}:
    get:
      summary: Get Users User Favorites Users Target User
      description: Finds a favorite user for a user
      operationId: getUsersUserFavoritesUsersTargetUser
      x-api-path-slug: usersuser-idfavoritesuserstarget-user-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Users
      - Target
      - User
    post:
      summary: Post Users User Favorites Users Target User
      description: Creates a new favorite listing for a user
      operationId: postUsersUserFavoritesUsersTargetUser
      x-api-path-slug: usersuser-idfavoritesuserstarget-user-id-post
      parameters:
      - in: query
        name: target_user_id
      - in: query
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Users
      - Target
      - User
    delete:
      summary: Delete Users User Favorites Users Target User
      description: Delete a favorite listing for a user
      operationId: deleteUsersUserFavoritesUsersTargetUser
      x-api-path-slug: usersuser-idfavoritesuserstarget-user-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Users
      - Target
      - User
  /homepages/pickers/:
    get:
      summary: Get Homepages Pickers
      description: Finds all FeaturedListingPicker in scope active.
      operationId: getHomepagesPickers
      x-api-path-slug: homepagespickers-get
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Pickers
  /homepages/pickers/{featured_listing_picker_id}:
    get:
      summary: Get Homepages Pickers Featured Listing Picker
      description: Retrieves a FeaturedListingPicker by id.
      operationId: getHomepagesPickersFeaturedListingPicker
      x-api-path-slug: homepagespickersfeatured-listing-picker-id-get
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Pickers
      - Featured
      - Listing
      - Picker
  /homepages/pickers/{featured_listing_picker_id}/featured:
    get:
      summary: Get Homepages Pickers Featured Listing Picker Featured
      description: Retrieves a set of FeaturedListing objects associated to a FeaturedListingPicker.
      operationId: getHomepagesPickersFeaturedListingPickerFeatured
      x-api-path-slug: homepagespickersfeatured-listing-picker-idfeatured-get
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Pickers
      - Featured
      - Listing
      - Picker
      - Featured
  /homepages/pickers/{featured_listing_picker_id}/listings:
    get:
      summary: Get Homepages Pickers Featured Listing Picker Listings
      description: Retrieves a set of Listing objects associated to a FeaturedListingPicker.
      operationId: getHomepagesPickersFeaturedListingPickerListings
      x-api-path-slug: homepagespickersfeatured-listing-picker-idlistings-get
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Pickers
      - Featured
      - Listing
      - Picker
      - Listings
  /homepages/pickers/{featured_listing_picker_id}/listings/active:
    get:
      summary: Get Homepages Pickers Featured Listing Picker Listings Active
      description: Retrieves a set of Listing objects associated to a FeaturedListingPicker
        in scope active.
      operationId: getHomepagesPickersFeaturedListingPickerListingsActive
      x-api-path-slug: homepagespickersfeatured-listing-picker-idlistingsactive-get
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Pickers
      - Featured
      - Listing
      - Picker
      - Listings
      - Active
  /homepages/listings/:
    get:
      summary: Get Homepages Listings
      description: Finds all FeaturedListings regardless of Listing state
      operationId: getHomepagesListings
      x-api-path-slug: homepageslistings-get
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Listings
  /homepages/listings/active:
    get:
      summary: Get Homepages Listings Active
      description: Finds all FeaturedListings that point to active Listings
      operationId: getHomepagesListingsActive
      x-api-path-slug: homepageslistingsactive-get
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Listings
      - Active
  /homepages/listings/{featured_listing_id}:
    get:
      summary: Get Homepages Listings Featured Listing
      description: Retrieves a FeaturedListing by id.
      operationId: getHomepagesListingsFeaturedListing
      x-api-path-slug: homepageslistingsfeatured-listing-id-get
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Listings
      - Featured
      - Listing
  /homepages/listings/{featured_listing_id}/picker:
    get:
      summary: Get Homepages Listings Featured Listing Picker
      description: Retrieves a set of FeaturedListingPicker objects associated to
        a FeaturedListing.
      operationId: getHomepagesListingsFeaturedListingPicker
      x-api-path-slug: homepageslistingsfeatured-listing-idpicker-get
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Listings
      - Featured
      - Listing
      - Picker
  /homepages/listings/{featured_listing_id}/listing:
    get:
      summary: Get Homepages Listings Featured Listing Listing
      description: Retrieves a set of Listing objects associated to a FeaturedListing.
      operationId: getHomepagesListingsFeaturedListingListing
      x-api-path-slug: homepageslistingsfeatured-listing-idlisting-get
      responses:
        200:
          description: OK
      tags:
      - Home Pages
      - Listings
      - Featured
      - Listing
      - Listing
  /listings/{listing_id}/images/{listing_image_id}:
    get:
      summary: Get Listings Listing Images Listing Image
      description: Retrieves a ListingImage by id.
      operationId: getListingsListingImagesListingImage
      x-api-path-slug: listingslisting-idimageslisting-image-id-get
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Images
      - Listing
      - Image
    delete:
      summary: Delete Listings Listing Images Listing Image
      description: Deletes a listing image
      operationId: deleteListingsListingImagesListingImage
      x-api-path-slug: listingslisting-idimageslisting-image-id-delete
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Images
      - Listing
      - Image
  /listings/{listing_id}/images:
    post:
      summary: Post Listings Listing Images
      description: Upload a new listing image
      operationId: postListingsListingImages
      x-api-path-slug: listingslisting-idimages-post
      parameters:
      - in: query
        name: image
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Images
    get:
      summary: Get Listings Listing Images
      description: Retrieves a set of ListingImage objects associated to a Listing.
      operationId: getListingsListingImages
      x-api-path-slug: listingslisting-idimages-get
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Images
  /listings/{listing_id}:
    get:
      summary: Get Listings Listing
      description: Retrieves a Listing by id.
      operationId: getListingsListing
      x-api-path-slug: listingslisting-id-get
      responses:
        200:
          description: OK
      tags:
      - Listings
    put:
      summary: Put Listings Listing
      description: Updates a Listing
      operationId: putListingsListing
      x-api-path-slug: listingslisting-id-put
      parameters:
      - in: query
        name: description
      - in: query
        name: materials
      - in: query
        name: price
      - in: query
        name: quantity
      - in: query
        name: renew
      - in: query
        name: shipping_template_id
      - in: query
        name: shop_section_id
      - in: query
        name: state
      - in: query
        name: tags
      - in: query
        name: title
      responses:
        200:
          description: OK
      tags:
      - Listings
    delete:
      summary: Delete Listings Listing
      description: Deletes a Listing
      operationId: deleteListingsListing
      x-api-path-slug: listingslisting-id-delete
      responses:
        200:
          description: OK
      tags:
      - Listings
  /listings/{listing_id}/favored-by:
    get:
      summary: Get Listings Listing Favored By
      description: Retrieves a set of FavoriteListing objects associated to a Listing.
      operationId: getListingsListingFavoredBy
      x-api-path-slug: listingslisting-idfavoredby-get
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Favored-by
  /listings/{listing_id}/shipping/info:
    get:
      summary: Get Listings Listing Shipping Info
      description: Retrieves a set of ShippingInfo objects associated to a Listing.
      operationId: getListingsListingShippingInfo
      x-api-path-slug: listingslisting-idshippinginfo-get
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Shipping
      - Info
    post:
      summary: Post Listings Listing Shipping Info
      description: Creates a new ShippingInfo.
      operationId: postListingsListingShippingInfo
      x-api-path-slug: listingslisting-idshippinginfo-post
      parameters:
      - in: query
        name: destination_country_id
      - in: query
        name: origin_country_id
      - in: query
        name: primary_cost
      - in: query
        name: region_id
      - in: query
        name: secondary_cost
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Shipping
      - Info
  /listings/{listing_id}/payments:
    get:
      summary: Get Listings Listing Payments
      description: Retrieves a set of ListingPayment objects associated to a Listing.
      operationId: getListingsListingPayments
      x-api-path-slug: listingslisting-idpayments-get
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Payments
  /listings/active:
    get:
      summary: Get Listings Active
      description: Finds all active Listing
      operationId: getListingsActive
      x-api-path-slug: listingsactive-get
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Active
  /shops/{shop_id}/listings/active:
    get:
      summary: Get Shops Shop Listings Active
      description: Finds all active Listings associated with a Shop
      operationId: getShopsShopListingsActive
      x-api-path-slug: shopsshop-idlistingsactive-get
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Listings
      - Active
  /listings:
    post:
      summary: Post Listings
      description: Creates a new Listing
      operationId: postListings
      x-api-path-slug: listings-post
      parameters:
      - in: query
        name: description
      - in: query
        name: materials
      - in: query
        name: price
      - in: query
        name: quantity
      - in: query
        name: shipping_template_id
      - in: query
        name: shop_section_id
      - in: query
        name: tags
      - in: query
        name: title
      responses:
        200:
          description: OK
      tags:
      - Listings
  /orders/{order_id}:
    get:
      summary: Get Orders Order
      description: Retrieves a Order by id.
      operationId: getOrdersOrder
      x-api-path-slug: ordersorder-id-get
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Order
  /orders/{order_id}/receipts:
    get:
      summary: Get Orders Order Receipts
      description: Retrieves a set of Receipt objects associated to a Order.
      operationId: getOrdersOrderReceipts
      x-api-path-slug: ordersorder-idreceipts-get
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Order
      - Receipts
  /receipts/{receipt_id}:
    get:
      summary: Get Receipts Receipt
      description: Retrieves a Receipt by id.
      operationId: getReceiptsReceipt
      x-api-path-slug: receiptsreceipt-id-get
      responses:
        200:
          description: OK
      tags:
      - Receipts
      - Receipt
    put:
      summary: Put Receipts Receipt
      description: Updates a Receipt
      operationId: putReceiptsReceipt
      x-api-path-slug: receiptsreceipt-id-put
      parameters:
      - in: query
        name: message_from_buyer
      - in: query
        name: message_from_seller
      - in: query
        name: receipt_id
      - in: query
        name: was_paid
      - in: query
        name: was_shipped
      responses:
        200:
          description: OK
      tags:
      - Receipts
      - Receipt
  /receipts/{receipt_id}/transactions:
    get:
      summary: Get Receipts Receipt Transactions
      description: Retrieves a set of Transaction objects associated to a Receipt.
      operationId: getReceiptsReceiptTransactions
      x-api-path-slug: receiptsreceipt-idtransactions-get
      responses:
        200:
          description: OK
      tags:
      - Receipts
      - Receipt
      - Transactions
  /users/{user_id}/recommended_listings:
    get:
      summary: Get Users User Recommended Listings
      description: Get recommended listings for an authenticated member. The number
        of listings returned may not match the specified limit if there is no activity
        from recommended shops.
      operationId: getUsersUserRecommendedListings
      x-api-path-slug: usersuser-idrecommended-listings-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Recommended
      - Listings
  /users/{user_id}/recommended_listings/rejects/{listing_ids}:
    post:
      summary: Post Users User Recommended Listings Rejects Listing S
      description: Registers rejections of recommended listings. Affects future recommended
        listings.
      operationId: postUsersUserRecommendedListingsRejectsListingS
      x-api-path-slug: usersuser-idrecommended-listingsrejectslisting-ids-post
      responses:
        200:
          description: OK
      tags:
      - Users
      - Recommended
      - Listings
      - Rejects
      - Listings
  /users/{user_id}/recommended_listings/views/{listing_ids}:
    post:
      summary: Post Users User Recommended Listings Views Listing S
      description: Register viewings of recommended listings. Affects future recommended
        listings.
      operationId: postUsersUserRecommendedListingsViewsListingS
      x-api-path-slug: usersuser-idrecommended-listingsviewslisting-ids-post
      responses:
        200:
          description: OK
      tags:
      - Users
      - Recommended
      - Listings
      - Views
      - Listings
  /regions/{region_id}:
    get:
      summary: Get Regions Region
      description: Retrieves a Region by id.
      operationId: getRegionsRegion
      x-api-path-slug: regionsregion-id-get
      responses:
        200:
          description: OK
      tags:
      - Regions
      - Region
  /regions:
    get:
      summary: Get Regions
      description: Finds all Region.
      operationId: getRegions
      x-api-path-slug: regions-get
      responses:
        200:
          description: OK
      tags:
      - Regions
  /shipping/info/{shipping_info_id}:
    get:
      summary: Get Shipping Info Shipping Info
      description: Retrieves a ShippingInfo by id.
      operationId: getShippingInfoShippingInfo
      x-api-path-slug: shippinginfoshipping-info-id-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Info
      - Shipping
      - Info
    put:
      summary: Put Shipping Info Shipping Info
      description: Updates a ShippingInfo with the given id.
      operationId: putShippingInfoShippingInfo
      x-api-path-slug: shippinginfoshipping-info-id-put
      parameters:
      - in: query
        name: destination_country_id
      - in: query
        name: listing_id
      - in: query
        name: origin_country_id
      - in: query
        name: primary_cost
      - in: query
        name: region_id
      - in: query
        name: secondary_cost
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Info
      - Shipping
      - Info
    delete:
      summary: Delete Shipping Info Shipping Info
      description: Deletes the ShippingInfo with the given id.
      operationId: deleteShippingInfoShippingInfo
      x-api-path-slug: shippinginfoshipping-info-id-delete
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Info
      - Shipping
      - Info
  /shipping/templates/entries/{shipping_template_entry_id}:
    get:
      summary: Get Shipping Templates Entries Shipping Template Entry
      description: Retrieves a ShippingTemplateEntry by id.
      operationId: getShippingTemplatesEntriesShippingTemplateEntry
      x-api-path-slug: shippingtemplatesentriesshipping-template-entry-id-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Entries
      - Shipping
      - Template
      - Entry
    put:
      summary: Put Shipping Templates Entries Shipping Template Entry
      description: Updates a ShippingTemplateEntry
      operationId: putShippingTemplatesEntriesShippingTemplateEntry
      x-api-path-slug: shippingtemplatesentriesshipping-template-entry-id-put
      parameters:
      - in: query
        name: destination_country_id
      - in: query
        name: primary_cost
      - in: query
        name: secondary_cost
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Entries
      - Shipping
      - Template
      - Entry
    delete:
      summary: Delete Shipping Templates Entries Shipping Template Entry
      description: Deletes a ShippingTemplateEntry
      operationId: deleteShippingTemplatesEntriesShippingTemplateEntry
      x-api-path-slug: shippingtemplatesentriesshipping-template-entry-id-delete
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Entries
      - Shipping
      - Template
      - Entry
  /shipping/templates/entries:
    post:
      summary: Post Shipping Templates Entries
      description: Creates a new ShippingTemplateEntry
      operationId: postShippingTemplatesEntries
      x-api-path-slug: shippingtemplatesentries-post
      parameters:
      - in: query
        name: destination_country_id
      - in: query
        name: destination_region_id
      - in: query
        name: primary_cost
      - in: query
        name: secondary_cost
      - in: query
        name: shipping_template_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Entries
  /shipping/templates/{shipping_template_id}:
    get:
      summary: Get Shipping Templates Shipping Template
      description: Retrieves a ShippingTemplate by id.
      operationId: getShippingTemplatesShippingTemplate
      x-api-path-slug: shippingtemplatesshipping-template-id-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Shipping
      - Template
    delete:
      summary: Delete Shipping Templates Shipping Template
      description: Deletes the ShippingTemplate with the given id.
      operationId: deleteShippingTemplatesShippingTemplate
      x-api-path-slug: shippingtemplatesshipping-template-id-delete
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Shipping
      - Template
    put:
      summary: Put Shipping Templates Shipping Template
      description: Updates a ShippingTemplate
      operationId: putShippingTemplatesShippingTemplate
      x-api-path-slug: shippingtemplatesshipping-template-id-put
      parameters:
      - in: query
        name: origin_country_id
      - in: query
        name: title
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Shipping
      - Template
  /shipping/templates/{shipping_template_id}/entries:
    get:
      summary: Get Shipping Templates Shipping Template Entries
      description: Retrieves a set of ShippingTemplateEntry objects associated to
        a ShippingTemplate.
      operationId: getShippingTemplatesShippingTemplateEntries
      x-api-path-slug: shippingtemplatesshipping-template-identries-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Shipping
      - Template
      - Entries
  /shipping/templates:
    post:
      summary: Post Shipping Templates
      description: Creates a new ShippingTemplate
      operationId: postShippingTemplates
      x-api-path-slug: shippingtemplates-post
      parameters:
      - in: query
        name: destination_country_id
      - in: query
        name: destination_region_id
      - in: query
        name: origin_country_id
      - in: query
        name: primary_cost
      - in: query
        name: secondary_cost
      - in: query
        name: title
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
  /shops/{shop_id}:
    get:
      summary: Get Shops Shop
      description: Retrieves a Shop by id.
      operationId: getShopsShop
      x-api-path-slug: shopsshop-id-get
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
    put:
      summary: Put Shops Shop
      description: Updates a Shop
      operationId: putShopsShop
      x-api-path-slug: shopsshop-id-put
      parameters:
      - in: query
        name: alchemy_message
      - in: query
        name: announcement
      - in: query
        name: is_refusing_alchemy
      - in: query
        name: policy_additional
      - in: query
        name: policy_payment
      - in: query
        name: policy_refunds
      - in: query
        name: policy_shipping
      - in: query
        name: policy_welcome
      - in: query
        name: sale_message
      - in: query
        name: title
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
  /shops/{shop_id}/receipts:
    get:
      summary: Get Shops Shop Receipts
      description: Retrieves a set of Receipt objects associated to a Shop.
      operationId: getShopsShopReceipts
      x-api-path-slug: shopsshop-idreceipts-get
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Receipts
  /shops/{shop_id}/transactions:
    get:
      summary: Get Shops Shop Transactions
      description: Retrieves a set of Transaction objects associated to a Shop.
      operationId: getShopsShopTransactions
      x-api-path-slug: shopsshop-idtransactions-get
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Transactions
  /shops/{shop_id}/sections:
    get:
      summary: Get Shops Shop Sections
      description: Retrieves a set of ShopSection objects associated to a Shop.
      operationId: getShopsShopSections
      x-api-path-slug: shopsshop-idsections-get
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Sections
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---