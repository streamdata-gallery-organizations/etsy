{
  "info": {
    "name": "Etsy Post Shops Shop Appearance Banner",
    "_postman_id": "4b599ac6-b805-4697-9098-4009493fba93",
    "description": "Upload a new shop banner image",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "f1a03ca7-269f-446b-9b4c-766b5b7aae2f",
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
              "id": "0930ee8e-eb5c-416c-b8ab-2fef507afbad"
            }
          ]
        },
        {
          "id": "c6a2a4c4-081f-41fa-ab52-8284acecdf50",
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
              "id": "8662d835-f53d-4fe9-9d18-900cb16280ee"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "b24fe9a8-5606-462d-9443-b88d3a516873",
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
              "id": "233a8439-b728-47ab-b9b4-5cb55f947269"
            }
          ]
        },
        {
          "id": "d7359ce5-efe6-47b0-be15-ee0d451bbb1e",
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
              "id": "0742a6d7-30db-44e5-81c9-ade3e7aa3aab"
            }
          ]
        },
        {
          "id": "707329a6-4bf5-441f-a7e9-b13ed1c39e30",
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
              "id": "bf0198a9-fb83-49ee-b57d-08c14992f72d"
            }
          ]
        },
        {
          "id": "15daf8aa-5228-4826-8fe3-f8e7d99068cc",
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
              "id": "f60fa76b-5473-4bd0-8c5f-20517158e814"
            }
          ]
        },
        {
          "id": "bd8fa756-f769-4180-adbc-9312cf68737e",
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
              "id": "8e4f1401-7e39-4145-a96b-48a446fa1a54"
            }
          ]
        },
        {
          "id": "f48cb4b8-82e2-4877-828d-efe267ebb2a8",
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
              "id": "58ddead3-b877-4a8c-93b8-a07edcbb12c9"
            }
          ]
        },
        {
          "id": "0042ca3d-370a-447d-9b7b-240de1b287c0",
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
              "id": "ab88f0fd-d17e-47bb-9418-82371d11b7ec"
            }
          ]
        },
        {
          "id": "d7ee7fe4-42eb-47d2-b822-e875fa47f8f9",
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
              "id": "10775e0b-3cc7-4ea6-84cd-e7bb84654359"
            }
          ]
        },
        {
          "id": "45c6f6fd-e138-49d1-82d8-ac16e6bc0d86",
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
              "id": "337c4220-86c6-46b6-bb14-dc513bb94512"
            }
          ]
        },
        {
          "id": "550293d1-60b8-407f-8c3e-1faa779f89a8",
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
              "id": "037d2d1e-8159-438d-ae07-420708d7e8d6"
            }
          ]
        },
        {
          "id": "6ab4aea8-6258-4e73-a8ad-841f1ea0d983",
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
              "id": "1d9b3fa8-3f10-4cb7-9585-44179f387d85"
            }
          ]
        }
      ]
    },
    {
      "name": "Home Pages",
      "item": [
        {
          "id": "8f88bec8-be27-4454-b3c7-f5cf4fafb521",
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
              "id": "acf9289f-d8db-4b68-96cc-04d363e487dc"
            }
          ]
        },
        {
          "id": "9f9f0e76-bd6b-4872-b4dd-e29c855b8b3d",
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
              "id": "6f1a9f96-bc91-426e-a87e-5989fcdaaeff"
            }
          ]
        },
        {
          "id": "673ee20c-e99f-46ff-8dd3-ff41850f9d67",
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
              "id": "2ab0b4ba-a98a-45a0-bb0b-ba0cf1fae9e5"
            }
          ]
        },
        {
          "id": "4320de80-fd21-4b9f-ba8c-8ca2d6d46c2b",
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
              "id": "12747fe4-9b16-4cdb-9715-54aa9c6daac7"
            }
          ]
        },
        {
          "id": "dd4f25d9-156b-413d-91c4-74d94ff7a71c",
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
              "id": "31e4afd9-d6ab-4e1e-8b3a-fa51044952ce"
            }
          ]
        },
        {
          "id": "0d4914e6-6673-4048-bcee-5ce97a87e76a",
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
              "id": "8ac5aa5e-e8b2-4dde-bf85-9c7740bd5e6f"
            }
          ]
        },
        {
          "id": "ee38c8ec-295d-4640-9a49-034da8b98a11",
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
              "id": "d6092cba-a392-404e-964a-e72f56a31045"
            }
          ]
        },
        {
          "id": "a19126d3-d8c0-4313-8fa0-476cdd8076af",
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
              "id": "dcaec585-85b4-4c7d-b197-00a20afbbb91"
            }
          ]
        },
        {
          "id": "5778127e-47de-4263-992e-825a75694d26",
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
              "id": "cef153f0-b396-4160-87fd-8b1ee7210457"
            }
          ]
        },
        {
          "id": "fabce9b0-fab1-4acc-957e-76ef84a640ae",
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
              "id": "8e876691-0d56-4911-82f8-6721c7b4c97a"
            }
          ]
        }
      ]
    },
    {
      "name": "Listings",
      "item": [
        {
          "id": "367c77bc-5afb-4232-bdff-1af3609642ac",
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
              "id": "c6018229-1171-42aa-afb0-d539db4cefef"
            }
          ]
        },
        {
          "id": "f5058318-fc53-4a5e-aa72-b395e0dee6df",
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
              "id": "aeac49e6-ee9b-48e0-b284-ee2750ed2c49"
            }
          ]
        },
        {
          "id": "9d0b2b6e-2813-4262-836b-7808800b6b80",
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
              "id": "71518610-dfc3-46e2-865b-238c75ddfe3f"
            }
          ]
        },
        {
          "id": "1ec94492-5048-426c-a7e6-b1fa468147b9",
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
              "id": "a6897daf-66c4-4975-8db7-5f41f57b9952"
            }
          ]
        },
        {
          "id": "4a8a14c9-37d3-4311-afb1-b7c3de4c4d00",
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
              "id": "448a20a9-1dc7-48ec-9f80-d5014de9468c"
            }
          ]
        },
        {
          "id": "9f05356d-6a10-4826-9539-5fa1aa770ce0",
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
              "id": "f39f1f8f-3672-4687-98a7-441b35887fc7"
            }
          ]
        },
        {
          "id": "751e2f2c-53cd-4dfc-a19d-c2e2716bf24e",
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
              "id": "e0783c3f-0572-4474-b2c0-dd433172c761"
            }
          ]
        },
        {
          "id": "b9400a5a-cde0-46ba-ab52-9c782f7f92b0",
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
              "id": "dfea756f-4201-4991-9748-1c9616a50df1"
            }
          ]
        },
        {
          "id": "70b846c9-9981-4eae-a640-cf6208d25d4d",
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
              "id": "3c3a1556-550a-4282-9f14-14efe31b7388"
            }
          ]
        },
        {
          "id": "068e58ae-3c10-4a08-bb76-b9d1ac900a88",
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
              "id": "c253fc8b-d3ac-410e-a78f-2b5efc534950"
            }
          ]
        },
        {
          "id": "d55cb20b-19a3-4980-83f9-ba89208ce5fe",
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
              "id": "30087a8f-0d49-4f55-b8d2-a3afba71c525"
            }
          ]
        },
        {
          "id": "ea566d6f-d6f3-458b-b569-d308db65190f",
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
              "id": "7dbcba86-80f1-4d9e-a1c4-4185e9f6b8d1"
            }
          ]
        },
        {
          "id": "da602d8f-b69a-496a-a5af-20a7208aa3d6",
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
              "id": "1c67c247-6d46-406a-bdaf-32cd1ad5e11d"
            }
          ]
        }
      ]
    },
    {
      "name": "Shops",
      "item": [
        {
          "id": "2dc5a22e-65ab-43b1-8709-ae539416bb71",
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
              "id": "b58c61cd-ff3f-423b-83eb-292f54603995"
            }
          ]
        },
        {
          "id": "68650c6d-fcec-4636-bfeb-ed464970e384",
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
              "id": "dd13b6cd-82f3-477e-994e-04692faa8b60"
            }
          ]
        },
        {
          "id": "55879f87-1a6b-4ca8-97fc-fef96a49aa1e",
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
              "id": "bc3549b9-837b-407e-b5c9-ff0f5615aad9"
            }
          ]
        },
        {
          "id": "9146cd17-46d4-4e9a-ab22-458547f067be",
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
              "id": "7e83fd8d-6844-48aa-b3da-26003aeb5451"
            }
          ]
        },
        {
          "id": "9a6981f3-20e2-46b9-b9df-3dd2549350e1",
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
              "id": "6ebef241-3329-48d3-a9d4-5a38338b9c7f"
            }
          ]
        },
        {
          "id": "3be1243b-3553-48c1-9f4e-51a3b79c6375",
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
              "id": "b36134f9-1878-4232-8572-97d4f847862a"
            }
          ]
        },
        {
          "id": "ab1791ab-51dd-4a32-8e49-495b36bfd335",
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
              "id": "fe2e2df9-253c-43e3-a336-cc146cbbf923"
            }
          ]
        },
        {
          "id": "806bf9ba-2e86-4201-b0f8-eb72c58840dc",
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
              "id": "60a4c96d-67eb-4e25-84d2-b03aaa0169f4"
            }
          ]
        },
        {
          "id": "e062e4ed-fba2-433c-bf25-4f10fced53cb",
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
              "id": "204ea03c-b2e7-457c-b67c-21b6b0f8d18e"
            }
          ]
        },
        {
          "id": "e912a0c6-6be0-40f0-a6b0-c306c02c14ab",
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
              "id": "9c83a786-7631-440b-8f03-51aa8c92cb2a"
            }
          ]
        },
        {
          "id": "fe512349-0f2f-4187-8eb6-ecdba79e77e7",
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
              "id": "2ac545d5-e669-4d0c-97fe-ce75bb23bee1"
            }
          ]
        },
        {
          "id": "abd6dd4f-8ab3-4c3f-9390-93e8c41a0e75",
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
              "id": "ebac082b-1362-4ae1-ba86-3f2c6452eae9"
            }
          ]
        },
        {
          "id": "93634f34-ea6c-4a1c-a6b3-206347dfb5b0",
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
              "id": "9ea65fdc-92ad-4f30-8f56-a73cd8d15eb8"
            }
          ]
        }
      ]
    },
    {
      "name": "Orders",
      "item": [
        {
          "id": "7040e74d-2e79-418d-a312-1267338c5b0d",
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
              "id": "960fa10c-0a02-4926-87b8-2676869b8a57"
            }
          ]
        },
        {
          "id": "ab6623f5-9d4e-4097-a30e-fc36fab4c21a",
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
              "id": "23e3b772-3958-4a9e-8dbe-06f35e275a8e"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipts",
      "item": [
        {
          "id": "3a264c65-0cb5-4b12-a8f7-8dd94bdeb72d",
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
              "id": "d6c6c3a2-b2c8-4a67-81e1-fb04f1ff5444"
            }
          ]
        },
        {
          "id": "a6592083-d455-4bba-81b9-7a8bb89feb82",
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
              "id": "be0d7df7-5dc9-486a-8fc5-e3377429f06f"
            }
          ]
        },
        {
          "id": "9a5c540b-ff35-484c-b032-04c8e8080cd8",
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
              "id": "7ddb41e4-110c-483e-a10d-f0195a1d0a51"
            }
          ]
        }
      ]
    },
    {
      "name": "Regions",
      "item": [
        {
          "id": "78a977d9-cfed-4e92-b2a9-0fd59df722c1",
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
              "id": "b47b4595-c4ff-4873-8655-845217c862a8"
            }
          ]
        },
        {
          "id": "8655e007-0844-436b-85de-aca2975809f2",
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
              "id": "8892a778-d054-4914-8ff0-04187b58a291"
            }
          ]
        }
      ]
    },
    {
      "name": "Shipping",
      "item": [
        {
          "id": "5780b50c-aaad-41b4-81b7-a577fc79beea",
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
              "id": "594c9557-4a95-40ef-a048-b96d9d9549d1"
            }
          ]
        },
        {
          "id": "487c4a84-3915-40a1-be81-594561d1cf30",
          "name": "putShippingInfoShippingInfo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shipping/info/:shipping_info_id"
              ],
              "query": [
                {
                  "key": "destination_country_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "listing_id",
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
                  "id": "shipping_info_id",
                  "value": "shipping_info_id",
                  "type":