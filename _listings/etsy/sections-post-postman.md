{
  "info": {
    "name": "Etsy Post Sections",
    "_postman_id": "f763562b-6872-47ba-a1a3-b79b95700eb9",
    "description": "Creates a new ShopSection.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "706b1008-a181-467d-a110-0ac828cd117a",
          "name": "getCountriesCountry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "countries/:country_id"
              ],
              "variable": [
                {
                  "id": "country_id",
                  "value": "country_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Country by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "217d6083-f4b3-42b9-a1b4-2be716f70ba4"
            }
          ]
        },
        {
          "id": "001400bf-8451-44dd-9afa-a0f2a537415d",
          "name": "getCountries",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/countries",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all Country."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb4ec930-facc-4db8-b3f5-59e22435e86c"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "1be7e696-4dfc-4787-b95b-f3c1c6f7829e",
          "name": "getUsersUserFavoritesListings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/listings"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all favorite listings for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93c737e4-d5da-408d-a7f4-9c3e55cb9484"
            }
          ]
        },
        {
          "id": "8d84821a-072b-4ff7-8784-1e0c802d4c98",
          "name": "getUsersUserFavoritesListingsListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/listings/:listing_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds a favorite listing for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1cffb8ee-0d63-46c1-8054-421f2e4aaf88"
            }
          ]
        },
        {
          "id": "08a6cb67-5435-43de-acb5-2001713a0786",
          "name": "postUsersUserFavoritesListingsListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/listings/:listing_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new favorite listing for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbde28cb-3915-46a2-abdb-c52fe8263424"
            }
          ]
        },
        {
          "id": "e0536f17-30a1-4607-9cca-4d66ff01585e",
          "name": "deleteUsersUserFavoritesListingsListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/listings/:listing_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a favorite listing for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d673ceb4-6027-4128-a69f-e27827e0182f"
            }
          ]
        },
        {
          "id": "fa0ac674-ce8d-4db6-ade6-601d0bd927e2",
          "name": "getUsersUserFavoritesUsers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/users"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all favorite users for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4849384-fd76-4cff-a1d5-6db9eb1f45a9"
            }
          ]
        },
        {
          "id": "8833a8d3-78f5-4eb9-98fe-de4c6f534372",
          "name": "getUsersUserFavoritesUsersTargetUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/users/:target_user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "target_user_id",
                  "value": "target_user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds a favorite user for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "faba7600-f299-47ab-8f20-62d9813dde7d"
            }
          ]
        },
        {
          "id": "f21db63d-29de-4ffc-965e-616b8c8abeff",
          "name": "postUsersUserFavoritesUsersTargetUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/users/:target_user_id"
              ],
              "variable": [
                {
                  "id": "target_user_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new favorite listing for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c1b863a-3cc0-464d-baed-1bbc82d812cb"
            }
          ]
        },
        {
          "id": "61ef6b5a-304a-44e7-b2a8-089d4e368e75",
          "name": "deleteUsersUserFavoritesUsersTargetUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/users/:target_user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "target_user_id",
                  "value": "target_user_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a favorite listing for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "620aa64f-171f-4e87-bdf7-51bbe0041097"
            }
          ]
        },
        {
          "id": "4335f90b-ae9c-43f6-bdda-56b98a78d383",
          "name": "getUsersUserRecommendedListings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/recommended_listings"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get recommended listings for an authenticated member. The number of listings returned may not match the specified limit if there is no activity from recommended shops."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80000c8a-82da-44c9-944f-d9e4d84005b7"
            }
          ]
        },
        {
          "id": "09ccb2c7-c817-4a89-bd1c-1c91d03054de",
          "name": "postUsersUserRecommendedListingsRejectsListingS",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/recommended_listings/rejects/:listing_ids"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "listing_ids",
                  "value": "listing_ids",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Registers rejections of recommended listings. Affects future recommended listings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbc52856-706a-4470-b6d6-b41f70ce652d"
            }
          ]
        },
        {
          "id": "f38f5bbe-9c81-474d-839c-0ecf9d3afbbb",
          "name": "postUsersUserRecommendedListingsViewsListingS",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/recommended_listings/views/:listing_ids"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "listing_ids",
                  "value": "listing_ids",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Register viewings of recommended listings. Affects future recommended listings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9906142f-a481-48cf-abba-49586ea8a1fc"
            }
          ]
        }
      ]
    },
    {
      "name": "Home Pages",
      "item": [
        {
          "id": "7f338ebc-8ee0-4f65-bcf6-0b7f3d489ad0",
          "name": "getHomepagesPickers",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/homepages/pickers/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all FeaturedListingPicker in scope active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d90fdfa-28b9-4897-9762-c16407b3d783"
            }
          ]
        },
        {
          "id": "46fee92c-7075-4f99-995d-2e941e4d62a6",
          "name": "getHomepagesPickersFeaturedListingPicker",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/pickers/:featured_listing_picker_id"
              ],
              "variable": [
                {
                  "id": "featured_listing_picker_id",
                  "value": "featured_listing_picker_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a FeaturedListingPicker by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d47eb13d-ba47-4172-9e70-e0aa86427270"
            }
          ]
        },
        {
          "id": "1f039dee-0b9b-4a64-b4db-6dbf6ab6abb5",
          "name": "getHomepagesPickersFeaturedListingPickerFeatured",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/pickers/:featured_listing_picker_id/featured"
              ],
              "variable": [
                {
                  "id": "featured_listing_picker_id",
                  "value": "featured_listing_picker_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of FeaturedListing objects associated to a FeaturedListingPicker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "667aa61f-6ecd-4583-b808-eb60a3dab744"
            }
          ]
        },
        {
          "id": "04eb5cf5-ff29-483c-beda-e07da82a7612",
          "name": "getHomepagesPickersFeaturedListingPickerListings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/pickers/:featured_listing_picker_id/listings"
              ],
              "variable": [
                {
                  "id": "featured_listing_picker_id",
                  "value": "featured_listing_picker_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Listing objects associated to a FeaturedListingPicker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f19e960-7081-4c8e-8027-ac80f903d972"
            }
          ]
        },
        {
          "id": "a19364ee-65c5-4131-b0dc-a95139efe440",
          "name": "getHomepagesPickersFeaturedListingPickerListingsActive",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/pickers/:featured_listing_picker_id/listings/active"
              ],
              "variable": [
                {
                  "id": "featured_listing_picker_id",
                  "value": "featured_listing_picker_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Listing objects associated to a FeaturedListingPicker in scope active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8a46373-cde3-420b-b6e3-5600265b1889"
            }
          ]
        },
        {
          "id": "46fbf8bc-9ab6-4400-a9f0-6edfae3508be",
          "name": "getHomepagesListings",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/homepages/listings/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all FeaturedListings regardless of Listing state"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b0f70ce-69b9-41d7-9176-cfd7c10bf81c"
            }
          ]
        },
        {
          "id": "9ebddb1e-1db9-472a-8473-9cb0aaf1b092",
          "name": "getHomepagesListingsActive",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/homepages/listings/active",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all FeaturedListings that point to active Listings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb0f09e4-0c22-45ad-8058-d7b8a1aa01fc"
            }
          ]
        },
        {
          "id": "b6450d39-1ebd-48c0-928a-1eb8905358aa",
          "name": "getHomepagesListingsFeaturedListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/listings/:featured_listing_id"
              ],
              "variable": [
                {
                  "id": "featured_listing_id",
                  "value": "featured_listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a FeaturedListing by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "804172ba-a421-4a4d-8316-fc4458c7151d"
            }
          ]
        },
        {
          "id": "313dd9ff-ef6b-4127-a851-11a94ce6c261",
          "name": "getHomepagesListingsFeaturedListingPicker",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/listings/:featured_listing_id/picker"
              ],
              "variable": [
                {
                  "id": "featured_listing_id",
                  "value": "featured_listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of FeaturedListingPicker objects associated to a FeaturedListing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d959ce3c-1785-4458-87d2-9f391ce847ab"
            }
          ]
        },
        {
          "id": "34fe1a0c-26ea-4cb8-871b-1fa11a57058f",
          "name": "getHomepagesListingsFeaturedListingListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/listings/:featured_listing_id/listing"
              ],
              "variable": [
                {
                  "id": "featured_listing_id",
                  "value": "featured_listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Listing objects associated to a FeaturedListing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58c4fe3f-f95d-47c5-ac7f-38f87c2876b4"
            }
          ]
        }
      ]
    },
    {
      "name": "Listings",
      "item": [
        {
          "id": "7b91b8cb-21b6-42e0-9514-e26690e1c758",
          "name": "getListingsListingImagesListingImage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/images/:listing_image_id"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                },
                {
                  "id": "listing_image_id",
                  "value": "listing_image_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a ListingImage by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcfae308-80b8-46da-b585-797f221b58a7"
            }
          ]
        },
        {
          "id": "4a0c43d9-6cb4-4c97-90a2-6b633ce6ba8d",
          "name": "deleteListingsListingImagesListingImage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/images/:listing_image_id"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                },
                {
                  "id": "listing_image_id",
                  "value": "listing_image_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a listing image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fba7145e-3833-402d-928d-e0fa16b0fc55"
            }
          ]
        },
        {
          "id": "9c6108dc-48a4-498f-833c-ce3cbe6e2421",
          "name": "getListingsListingImages",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/images"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of ListingImage objects associated to a Listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da05a7d5-bcb2-49e3-be87-37e8b98a5549"
            }
          ]
        },
        {
          "id": "725a05f3-f912-4769-8761-06b43840df77",
          "name": "postListingsListingImages",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/images"
              ],
              "query": [
                {
                  "key": "image",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload a new listing image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d770d1d5-2fa8-4812-8dd8-b3a88d8d2b96"
            }
          ]
        },
        {
          "id": "58e5b66f-c8d0-490c-8882-6ca776ec6e50",
          "name": "getListingsListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Listing by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c0b36fe-1d9f-4ce4-a345-9679519a60ce"
            }
          ]
        },
        {
          "id": "f9aecc0e-a1fb-4aeb-90f0-58a703ce2b22",
          "name": "putListingsListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id"
              ],
              "query": [
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "materials",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "price",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "quantity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "renew",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "shipping_template_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "shop_section_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a Listing"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e153102-ff01-4a95-b4a2-e481ab1ffc9c"
            }
          ]
        },
        {
          "id": "36312b2d-fd04-4988-8f18-63128b216bba",
          "name": "deleteListingsListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Listing"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5fbfad7-b30d-4fff-b98a-443144fbfd59"
            }
          ]
        },
        {
          "id": "7f26919c-32a9-49d3-99dd-abf1d7ba5289",
          "name": "getListingsListingFavoredBy",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/favored-by"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of FavoriteListing objects associated to a Listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8c525f8-7355-415e-afbf-a8bb4a76fa29"
            }
          ]
        },
        {
          "id": "97696b3f-3485-4701-b0e0-712cd1cdc10b",
          "name": "getListingsListingShippingInfo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/shipping/info"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of ShippingInfo objects associated to a Listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7caadf4b-8644-41cd-9c01-7fdbc63ba1e7"
            }
          ]
        },
        {
          "id": "286cb203-8168-4de9-9d9e-dcf2cdf1ba42",
          "name": "postListingsListingShippingInfo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/shipping/info"
              ],
              "query": [
                {
                  "key": "destination_country_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "origin_country_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "primary_cost",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "region_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "secondary_cost",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new ShippingInfo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8de84b6-4030-40d0-9250-c58d099ee0c6"
            }
          ]
        },
        {
          "id": "a3d364f6-0bc5-48e4-995c-106f93d5086a",
          "name": "getListingsListingPayments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/payments"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of ListingPayment objects associated to a Listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ae55dfc-3b51-4680-8d13-baa8b79e6a14"
            }
          ]
        },
        {
          "id": "73b1d7bc-3246-441a-a617-523cebad31bb",
          "name": "getListingsActive",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/listings/active",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all active Listing"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31262d4d-a099-428c-8c21-35c34efa43ce"
            }
          ]
        },
        {
          "id": "7f136414-d36e-4e21-ad55-72c339d547e7",
          "name": "postListings",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/listings?description=%7B%7D&materials=%7B%7D&price=%7B%7D&quantity=%7B%7D&shipping_template_id=%7B%7D&shop_section_id=%7B%7D&tags=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Listing"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f79bf5c-2730-4cea-8a39-65264aea062d"
            }
          ]
        }
      ]
    },
    {
      "name": "Shops",
      "item": [
        {
          "id": "bc920d66-a165-4022-aadb-1acb6994ee00",
          "name": "getShopsShopListingsActive",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/listings/active"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all active Listings associated with a Shop"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b0e00eb-bf8b-45d8-a112-36897f139d11"
            }
          ]
        },
        {
          "id": "2848ba4b-fa57-44cd-92a8-ce4601cbdde4",
          "name": "getShopsShop",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Shop by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e06f1309-c4b1-43cf-99d6-4bd2c323463f"
            }
          ]
        },
        {
          "id": "437539b3-8fce-478f-a49e-ef8f941076ed",
          "name": "putShopsShop",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id"
              ],
              "query": [
                {
                  "key": "alchemy_message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "announcement",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_refusing_alchemy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "policy_additional",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "policy_payment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "policy_refunds",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "policy_shipping",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "policy_welcome",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sale_message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a Shop"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ac406cd-d0f4-4585-a9dc-cef017336b79"
            }
          ]
        },
        {
          "id": "3c500317-47bb-4350-be73-381e6d9eb546",
          "name": "getShopsShopReceipts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/receipts"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Receipt objects associated to a Shop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f148628-0d86-4a7e-8b45-8e574d6ebd84"
            }
          ]
        },
        {
          "id": "2092dff9-15ec-47af-9b92-a08ccaf06d76",
          "name": "getShopsShopTransactions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/transactions"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Transaction objects associated to a Shop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cbd4c0b-596e-4ee0-8cca-64c2864d6dae"
            }
          ]
        },
        {
          "id": "cb60ab61-de04-45d5-84bc-f3ba2e0d2eff",
          "name": "getShopsShopSections",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/sections"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of ShopSection objects associated to a Shop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12b5c421-d777-4335-b8cf-72529610e658"
            }
          ]
        },
        {
          "id": "315a996b-3dde-41fa-8ffb-041185f6d61e",
          "name": "getShops",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/shops",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all Shops. If there is a keywords parameter, finds shops with shop_name starting with keywords."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd27e3e0-0838-4d6f-943d-75814a64a5cf"
            }
          ]
        },
        {
          "id": "87f722e3-1552-4022-9286-7659e46efc1d",
          "name": "getShopsShopListingsFeatured",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/listings/featured"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves Listings associated to a Shop that are featured"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88286a4b-e590-405d-875f-ab472d871b6f"
            }
          ]
        },
        {
          "id": "12a7462a-e388-4008-ac37-5f669458a7cc",
          "name": "getShopsShopListingsInactive",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/listings/inactive"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves Listings associated to a Shop that are inactive"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39a5b6ad-a2d8-4439-9a83-5d6db76207bf"
            }
          ]
        },
        {
          "id": "0c5bea9a-7cf2-4d12-941d-a449dfa17182",
          "name": "getShopsShopListingsExpired",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/listings/expired"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves Listings associated to a Shop that are expired"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be4a652b-57ef-4941-a310-74b766ac6ae4"
            }
          ]
        },
        {
          "id": "212f9be0-5d92-4589-9ccf-f22b97f47018",
          "name": "getShopsShopListingsInactiveListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/listings/inactive/:listing_id"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                },
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Listing associated to a Shop that is inactive"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7587790d-f0ec-446b-aa42-48fb76158068"
            }
          ]
        },
        {
          "id": "f170b42d-1daf-429a-ae51-d022ecff7159",
          "name": "getShopsShopListingsExpiredListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/listings/expired/:listing_id"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                },
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Listing associated to a Shop that is inactive"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f23aced5-5b7a-4240-afac-12993246a454"
            }
          ]
        },
        {
          "id": "012a4046-6657-468f-9855-5f44086f1adb",
          "name": "postShopsShopAppearanceBanner",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/appearance/banner"
              ],
              "query": [
                {
                  "key": "image",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload a new shop banner image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4d746fe-79f5-46ba-b92b-68d7b4e5d404"
            }
          ]
        },
        {
          "id": "9eb91f8a-8e23-4879-afb4-d8430eced7e2",
          "name": "deleteShopsShopAppearanceBannerShopBanner",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/appearance/banner/:shop_banner_id"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                },
                {
                  "id": "shop_banner_id",
                  "value": "shop_banner_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a shop banner image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b113d31b-5d84-455f-be77-1c3af08444a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Orders",
      "item": [
        {
          "id": "f37b3599-3188-4b97-a5ca-988afcd97fb8",
          "name": "getOrdersOrder",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "orders/:order_id"
              ],
              "variable": [
                {
                  "id": "order_id",
                  "value": "order_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Order by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba9e7aee-ccb3-4ce8-9fd3-5bd7b7ac4d72"
            }
          ]
        },
        {
          "id": "da5642ca-a285-49cf-979c-b2ddf2d0eca2",
          "name": "getOrdersOrderReceipts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "orders/:order_id/receipts"
              ],
              "variable": [
                {
                  "id": "order_id",
                  "value": "order_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Receipt objects associated to a Order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "998c168d-33a9-4fbc-9287-ec5e169c565c"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipts",
      "item": [
        {
          "id": "4d526aa3-f491-434b-bbfc-2a750e2ee913",
          "name": "getReceiptsReceipt",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "receipts/:receipt_id"
              ],
              "variable": [
                {
                  "id": "receipt_id",
                  "value": "receipt_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Receipt by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df60b09a-3b7d-4b0b-862a-030aff5abe89"
            }
          ]
        },
        {
          "id": "2ca11ce9-3ca1-46e3-9892-e0d3c39f9751",
          "name": "putReceiptsReceipt",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "receipts/:receipt_id"
              ],
              "query": [
                {
                  "key": "message_from_buyer",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message_from_seller",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "was_paid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "was_shipped",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "receipt_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a Receipt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e88f71fc-9d2f-4e02-af57-0c8984773ac5"
            }
          ]
        },
        {
          "id": "644bc9b3-30e1-4a05-b60c-5014a496c4c6",
          "name": "getReceiptsReceiptTransactions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "receipts/:receipt_id/transactions"
              ],
              "variable": [
                {
                  "id": "receipt_id",
                  "value": "receipt_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Transaction objects associated to a Receipt."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9a0ebf3-3dcd-4263-8d9f-349e3200cc5d"
            }
          ]
        }
      ]
    },
    {
      "name": "Regions",
      "item": [
        {
          "id": "a9ea79ad-1f2b-4738-a884-c35b7932e76c",
          "name": "getRegionsRegion",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "regions/:region_id"
              ],
              "variable": [
                {
                  "id": "region_id",
                  "value": "region_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Region by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef0589b4-0595-4e54-b4ad-9af3ab655c2b"
            }
          ]
        },
        {
          "id": "696c597a-82e4-4f04-85a8-4dd85620a962",
          "name": "getRegions",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/regions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all Region."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6932c7f-2ead-47d8-a4d6-061f2f0069fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Shipping",
      "item": [
        {
          "id": "3f9f9827-46ab-4b9b-9186-8697b524f834",
          "name": "getShippingInfoShippingInfo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shipping/info/:shipping_info_id"
              ],
              "variable": [
                {
                  "id": "shipping_info_id",
                  "value": "shipping_info_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a ShippingInfo by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1375e51-56c7-4a1a-b5f7-e67b2e3c6f75"
            }
          ]
        },
        {
          "id": "21d41224-32d5-4d07-8f7a-98083873a93a",
          "name": "putShippingInfoShippingInfo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shipping/info/:shipping_info_