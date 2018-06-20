---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Put Listings Listing
  description: Updates a Listing
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
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
      parameters:
      - in: path
        name: country_id
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
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
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
      parameters:
      - in: path
        name: listing_id
      - in: path
        name: user_id
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
      parameters:
      - in: path
        name: listing_id
      - in: path
        name: user_id
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
      parameters:
      - in: path
        name: listing_id
      - in: path
        name: user_id
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
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
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
      parameters:
      - in: path
        name: target_user_id
      - in: path
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
    post:
      summary: Post Users User Favorites Users Target User
      description: Creates a new favorite listing for a user
      operationId: postUsersUserFavoritesUsersTargetUser
      x-api-path-slug: usersuser-idfavoritesuserstarget-user-id-post
      parameters:
      - in: path
        name: target_user_id
      - in: query
        name: target_user_id
      - in: path
        name: user_id
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
      parameters:
      - in: path
        name: target_user_id
      - in: path
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
  /homepages/pickers/:
    get:
      summary: Get Homepages Pickers
      description: Finds all FeaturedListingPicker in scope active.
      operationId: getHomepagesPickers
      x-api-path-slug: homepagespickers-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
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
      parameters:
      - in: path
        name: featured_listing_picker_id
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
      parameters:
      - in: path
        name: featured_listing_picker_id
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
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
      parameters:
      - in: path
        name: featured_listing_picker_id
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
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
      parameters:
      - in: path
        name: featured_listing_picker_id
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
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
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
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
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
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
      parameters:
      - in: path
        name: featured_listing_id
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
      parameters:
      - in: path
        name: featured_listing_id
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
      parameters:
      - in: path
        name: featured_listing_id
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
      parameters:
      - in: path
        name: listing_id
      - in: path
        name: listing_image_id
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
      parameters:
      - in: path
        name: listing_id
      - in: path
        name: listing_image_id
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
      - in: path
        name: listing_id
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
      parameters:
      - in: path
        name: listing_id
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
      parameters:
      - in: path
        name: listing_id
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
      - in: path
        name: listing_id
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