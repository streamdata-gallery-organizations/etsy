---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Post Payments Templates
  description: Creates a new PaymentTemplate
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
  /shops:
    get:
      summary: Get Shops
      description: Finds all Shops. If there is a keywords parameter, finds shops
        with shop_name starting with keywords.
      operationId: getShops
      x-api-path-slug: shops-get
      responses:
        200:
          description: OK
      tags:
      - Shops
  /shops/{shop_id}/listings/featured:
    get:
      summary: Get Shops Shop Listings Featured
      description: Retrieves Listings associated to a Shop that are featured
      operationId: getShopsShopListingsFeatured
      x-api-path-slug: shopsshop-idlistingsfeatured-get
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Listings
      - Featured
  /shops/{shop_id}/listings/inactive:
    get:
      summary: Get Shops Shop Listings Inactive
      description: Retrieves Listings associated to a Shop that are inactive
      operationId: getShopsShopListingsInactive
      x-api-path-slug: shopsshop-idlistingsinactive-get
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Listings
      - Inactive
  /shops/{shop_id}/listings/expired:
    get:
      summary: Get Shops Shop Listings Expired
      description: Retrieves Listings associated to a Shop that are expired
      operationId: getShopsShopListingsExpired
      x-api-path-slug: shopsshop-idlistingsexpired-get
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Listings
      - Expired
  /shops/{shop_id}/listings/inactive/{listing_id}:
    get:
      summary: Get Shops Shop Listings Inactive Listing
      description: Retrieves a Listing associated to a Shop that is inactive
      operationId: getShopsShopListingsInactiveListing
      x-api-path-slug: shopsshop-idlistingsinactivelisting-id-get
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Listings
      - Inactive
      - Listing
  /shops/{shop_id}/listings/expired/{listing_id}:
    get:
      summary: Get Shops Shop Listings Expired Listing
      description: Retrieves a Listing associated to a Shop that is inactive
      operationId: getShopsShopListingsExpiredListing
      x-api-path-slug: shopsshop-idlistingsexpiredlisting-id-get
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Listings
      - Expired
      - Listing
  /shops/{shop_id}/appearance/banner:
    post:
      summary: Post Shops Shop Appearance Banner
      description: Upload a new shop banner image
      operationId: postShopsShopAppearanceBanner
      x-api-path-slug: shopsshop-idappearancebanner-post
      parameters:
      - in: query
        name: image
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Appearance
      - Banner
  /shops/{shop_id}/appearance/banner/{shop_banner_id}:
    delete:
      summary: Delete Shops Shop Appearance Banner Shop Banner
      description: Deletes a shop banner image
      operationId: deleteShopsShopAppearanceBannerShopBanner
      x-api-path-slug: shopsshop-idappearancebannershop-banner-id-delete
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Appearance
      - Banner
      - Shop
      - Banner
  /sections/{shop_section_id}:
    get:
      summary: Get Sections Shop Section
      description: Retrieves a ShopSection by id.
      operationId: getSectionsShopSection
      x-api-path-slug: sectionsshop-section-id-get
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Shop
      - Section
    put:
      summary: Put Sections Shop Section
      description: Updates a ShopSection with the given id.
      operationId: putSectionsShopSection
      x-api-path-slug: sectionsshop-section-id-put
      parameters:
      - in: query
        name: rank
      - in: query
        name: title
      - in: query
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Shop
      - Section
    delete:
      summary: Delete Sections Shop Section
      description: Deletes the ShopSection with the given id.
      operationId: deleteSectionsShopSection
      x-api-path-slug: sectionsshop-section-id-delete
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Shop
      - Section
  /sections:
    post:
      summary: Post Sections
      description: Creates a new ShopSection.
      operationId: postSections
      x-api-path-slug: sections-post
      parameters:
      - in: query
        name: title
      - in: query
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Sections
  /categories/{tag}:
    get:
      summary: Get Categories Tag
      description: Retrieves a top-level Category by tag.
      operationId: getCategoriesTag
      x-api-path-slug: categoriestag-get
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Tag
  /categories/{tag}/{subtag}:
    get:
      summary: Get Categories Tag Subtag
      description: Retrieves a second-level Category by tag and subtag.
      operationId: getCategoriesTagSubtag
      x-api-path-slug: categoriestagsubtag-get
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Tag
      - Subtag
  /categories/{tag}/{subtag}/{subsubtag}:
    get:
      summary: Get Categories Tag Subtag Subsubtag
      description: Retrieves a third-level Category by tag, subtag and subsubtag.
      operationId: getCategoriesTagSubtagSubsubtag
      x-api-path-slug: categoriestagsubtagsubsubtag-get
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Tag
      - Subtag
      - Subsubtag
  /taxonomy/categories:
    get:
      summary: Get Taxonomy Categories
      description: Retrieves all top-level Categories.
      operationId: getTaxonomyCategories
      x-api-path-slug: taxonomycategories-get
      responses:
        200:
          description: OK
      tags:
      - Taxonomy
      - Categories
  /taxonomy/categories/{tag}:
    get:
      summary: Get Taxonomy Categories Tag
      description: Retrieves children of a top-level Category by tag.
      operationId: getTaxonomyCategoriesTag
      x-api-path-slug: taxonomycategoriestag-get
      responses:
        200:
          description: OK
      tags:
      - Taxonomy
      - Categories
      - Tag
  /taxonomy/categories/{tag}/{subtag}:
    get:
      summary: Get Taxonomy Categories Tag Subtag
      description: Retrieves children of a second-level Category by tag and subtag.
      operationId: getTaxonomyCategoriesTagSubtag
      x-api-path-slug: taxonomycategoriestagsubtag-get
      responses:
        200:
          description: OK
      tags:
      - Taxonomy
      - Categories
      - Tag
      - Subtag
  /taxonomy/tags:
    get:
      summary: Get Taxonomy Tags
      description: Retrieves all related tags for the given tag set.
      operationId: getTaxonomyTags
      x-api-path-slug: taxonomytags-get
      responses:
        200:
          description: OK
      tags:
      - Taxonomy
      - Tags
  /taxonomy/tags/{tags}:
    get:
      summary: Get Taxonomy Tags Tags
      description: Retrieves all related tags for the given tag set.
      operationId: getTaxonomyTagsTags
      x-api-path-slug: taxonomytagstags-get
      responses:
        200:
          description: OK
      tags:
      - Taxonomy
      - Tags
      - Tags
  /transactions/{transaction_id}:
    get:
      summary: Get Transactions Transaction
      description: Retrieves a Transaction by id.
      operationId: getTransactionsTransaction
      x-api-path-slug: transactionstransaction-id-get
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Transaction
  /treasuries/{treasury_id}:
    get:
      summary: Get Treasuries Treasury
      description: Get a Treasury
      operationId: getTreasuriesTreasury
      x-api-path-slug: treasuriestreasury-id-get
      responses:
        200:
          description: OK
      tags:
      - Treasuries
  /treasuries:
    get:
      summary: Get Treasuries
      description: Search Treasuries or else List all Treasuries
      operationId: getTreasuries
      x-api-path-slug: treasuries-get
      responses:
        200:
          description: OK
      tags:
      - Treasuries
  /users/{user_id}/treasuries:
    get:
      summary: Get Users User Treasuries
      description: Get a user's Treasuries
      operationId: getUsersUserTreasuries
      x-api-path-slug: usersuser-idtreasuries-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Treasuries
  /users/{user_id}:
    get:
      summary: Get Users User
      description: Retrieves a User by id.
      operationId: getUsersUser
      x-api-path-slug: usersuser-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{user_id}/shops:
    get:
      summary: Get Users User Shops
      description: Retrieves a set of Shop objects associated to a User.
      operationId: getUsersUserShops
      x-api-path-slug: usersuser-idshops-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Shops
  /users/{user_id}/favored-by:
    get:
      summary: Get Users User Favored By
      description: Retrieves a set of FavoriteUser objects associated to a User.
      operationId: getUsersUserFavoredBy
      x-api-path-slug: usersuser-idfavoredby-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favored-by
  /users/{user_id}/feedback/as-subject:
    get:
      summary: Get Users User Feedback As Subject
      description: Retrieves a set of Feedback objects associated to a User.
      operationId: getUsersUserFeedbackAsSubject
      x-api-path-slug: usersuser-idfeedbackassubject-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Feedback
      - As-subject
  /users/{user_id}/feedback/as-author:
    get:
      summary: Get Users User Feedback As Author
      description: Retrieves a set of Feedback objects associated to a User.
      operationId: getUsersUserFeedbackAsAuthor
      x-api-path-slug: usersuser-idfeedbackasauthor-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Feedback
      - As-author
  /users/{user_id}/feedback/as-buyer:
    get:
      summary: Get Users User Feedback As Buyer
      description: Retrieves a set of Feedback objects associated to a User.
      operationId: getUsersUserFeedbackAsBuyer
      x-api-path-slug: usersuser-idfeedbackasbuyer-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Feedback
      - As-buyer
  /users/{user_id}/feedback/as-seller:
    get:
      summary: Get Users User Feedback As Seller
      description: Retrieves a set of Feedback objects associated to a User.
      operationId: getUsersUserFeedbackAsSeller
      x-api-path-slug: usersuser-idfeedbackasseller-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Feedback
      - As-seller
  /users/{user_id}/orders:
    get:
      summary: Get Users User Orders
      description: Retrieves a set of Order objects associated to a User.
      operationId: getUsersUserOrders
      x-api-path-slug: usersuser-idorders-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Orders
  /users/{user_id}/receipts:
    get:
      summary: Get Users User Receipts
      description: Retrieves a set of Receipt objects associated to a User.
      operationId: getUsersUserReceipts
      x-api-path-slug: usersuser-idreceipts-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Receipts
  /users/{user_id}/transactions:
    get:
      summary: Get Users User Transactions
      description: Retrieves a set of Transaction objects associated to a User.
      operationId: getUsersUserTransactions
      x-api-path-slug: usersuser-idtransactions-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Transactions
  /users/{user_id}/charges:
    get:
      summary: Get Users User Charges
      description: Retrieves a set of BillCharge objects associated to a User.
      operationId: getUsersUserCharges
      x-api-path-slug: usersuser-idcharges-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Charges
  /users/{user_id}/payments:
    get:
      summary: Get Users User Payments
      description: Retrieves a set of BillPayment objects associated to a User.
      operationId: getUsersUserPayments
      x-api-path-slug: usersuser-idpayments-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Payments
  /users/{user_id}/shipping/templates:
    get:
      summary: Get Users User Shipping Templates
      description: Retrieves a set of ShippingTemplate objects associated to a User.
      operationId: getUsersUserShippingTemplates
      x-api-path-slug: usersuser-idshippingtemplates-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Shipping
      - Templates
  /users/{user_id}/payments/templates:
    get:
      summary: Get Users User Payments Templates
      description: Retrieves a set of PaymentTemplate objects associated to a User.
      operationId: getUsersUserPaymentsTemplates
      x-api-path-slug: usersuser-idpaymentstemplates-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Payments
      - Templates
  /users/{user_id}/addresses:
    get:
      summary: Get Users User Addresses
      description: Retrieves a set of UserAddress objects associated to a User.
      operationId: getUsersUserAddresses
      x-api-path-slug: usersuser-idaddresses-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Addresses
    post:
      summary: Post Users User Addresses
      description: Creates a new UserAddress.
      operationId: postUsersUserAddresses
      x-api-path-slug: usersuser-idaddresses-post
      parameters:
      - in: query
        name: city
      - in: query
        name: country_id
      - in: query
        name: first_line
      - in: query
        name: name
      - in: query
        name: second_line
      - in: query
        name: state
      - in: query
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Users
      - Addresses
  /payments/templates/{payment_template_id}:
    get:
      summary: Get Payments Templates Payment Template
      description: Retrieves a PaymentTemplate by id.
      operationId: getPaymentsTemplatesPaymentTemplate
      x-api-path-slug: paymentstemplatespayment-template-id-get
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Templates
      - Payment
      - Template
    put:
      summary: Put Payments Templates Payment Template
      description: Updates a PaymentTemplate
      operationId: putPaymentsTemplatesPaymentTemplate
      x-api-path-slug: paymentstemplatespayment-template-id-put
      parameters:
      - in: query
        name: allow_check
      - in: query
        name: allow_mo
      - in: query
        name: allow_other
      - in: query
        name: allow_paypal
      - in: query
        name: city
      - in: query
        name: country_id
      - in: query
        name: first_line
      - in: query
        name: name
      - in: query
        name: paypal_email
      - in: query
        name: second_line
      - in: query
        name: state
      - in: query
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Templates
      - Payment
      - Template
  /payments/templates:
    post:
      summary: Post Payments Templates
      description: Creates a new PaymentTemplate
      operationId: postPaymentsTemplates
      x-api-path-slug: paymentstemplates-post
      parameters:
      - in: query
        name: allow_check
      - in: query
        name: allow_mo
      - in: query
        name: allow_other
      - in: query
        name: allow_paypal
      - in: query
        name: city
      - in: query
        name: country_id
      - in: query
        name: first_line
      - in: query
        name: name
      - in: query
        name: paypal_email
      - in: query
        name: second_line
      - in: query
        name: state
      - in: query
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Templates
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