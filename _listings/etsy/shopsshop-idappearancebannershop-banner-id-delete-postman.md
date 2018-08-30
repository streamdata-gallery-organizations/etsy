{
  "info": {
    "name": "Etsy Delete Shops Shop Appearance Banner Shop Banner",
    "_postman_id": "c8ed3323-4fcb-478e-8042-806673a7eada",
    "description": "Deletes a shop banner image",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "66476453-32d4-449b-9185-7de62d207eab",
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
              "id": "c64937d0-a214-4662-80ed-fba500f11c26"
            }
          ]
        },
        {
          "id": "e401ddab-a2c5-4769-b476-f1a444cf735c",
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
              "id": "04fcca13-ebf0-475f-ba02-89218f73b152"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "82c6deda-f684-417e-b321-ef021f89c2b1",
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
              "id": "315a185e-24bf-4734-b601-99dc110a4861"
            }
          ]
        },
        {
          "id": "4c6baf28-85ea-4f22-ac13-3b0c2f33e3b6",
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
              "id": "72a3c373-7e68-4439-b320-198516b4517e"
            }
          ]
        },
        {
          "id": "2a6594f7-648c-429c-b96e-a5575f0dd852",
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
              "id": "eebaa00c-f8d1-45ee-acc7-b68610d626ef"
            }
          ]
        },
        {
          "id": "d155025d-5814-4649-a303-5ec6f0059952",
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
              "id": "efdeb9c1-bef1-47eb-a738-cfadc5bdc0dd"
            }
          ]
        },
        {
          "id": "a592a1f3-e74c-4229-ae77-7183db928b44",
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
              "id": "b69ccb4e-315e-490c-877a-ebd374dc48e1"
            }
          ]
        },
        {
          "id": "bd712612-6bc5-4e63-acbf-892a3a26d9dd",
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
              "id": "2f5fc96b-0157-4c99-b4cb-52da67ee3aea"
            }
          ]
        },
        {
          "id": "73482ca4-6891-4fab-b133-69ad7961b599",
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
              "id": "0aaac1e3-712a-4a94-8bec-dd09dc9fecfd"
            }
          ]
        },
        {
          "id": "f4709468-a347-4875-ac62-727f63442a78",
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
              "id": "0d5d4914-b44f-4e93-af01-0aa986e0b967"
            }
          ]
        },
        {
          "id": "4bfc87fb-5aba-4787-8a67-b9cddf9e1cd5",
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
              "id": "01690aad-6f5f-4c44-a2e8-48aa58969552"
            }
          ]
        },
        {
          "id": "a9600d13-f803-4a12-aecd-7a8b27a88a25",
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
              "id": "5bedfca1-2aee-433a-8294-d9deb52571c6"
            }
          ]
        },
        {
          "id": "31fa10c8-40df-44ad-9f00-5e2718d55a47",
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
              "id": "7559cd3f-4233-449b-b421-cfbc7950d3f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Home Pages",
      "item": [
        {
          "id": "f023bd66-f392-47a6-b7ce-486769e1e47a",
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
              "id": "751399c1-9e6b-4f57-b6c1-24354d0354bb"
            }
          ]
        },
        {
          "id": "9991dabd-ecaa-4e70-aa24-949374d934ce",
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
              "id": "0b348525-d77b-4d6f-bb62-674d9f4dcb75"
            }
          ]
        },
        {
          "id": "ba5bcc43-9ecc-4404-bf64-7ae6ec826a7c",
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
              "id": "a311cbff-70de-4124-8659-15a9ea8d7881"
            }
          ]
        },
        {
          "id": "de673d02-1627-48d2-9491-ed9ce957c2de",
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
              "id": "a4a07238-bca0-43bd-a2df-f22c6d43fdd8"
            }
          ]
        },
        {
          "id": "1d19245f-e9d5-4280-b2f4-e6da4fc00d15",
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
              "id": "bd866e50-b6be-456f-99a4-21378c9883ad"
            }
          ]
        },
        {
          "id": "3cb86eac-0e78-4042-bf3d-dc0ffd3c1c58",
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
              "id": "75bbb597-7454-4cb9-b7f5-621c10d00428"
            }
          ]
        },
        {
          "id": "13d22ecd-a68a-4e20-9ab2-cf8cc71b3888",
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
              "id": "77fd4e23-4afb-4ffb-bf10-7dbe6bb54090"
            }
          ]
        },
        {
          "id": "f0ed06ab-31fc-4651-93c1-441fc892f943",
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
              "id": "7cc6efae-755e-40d7-b2f7-aa2c4bfc77c0"
            }
          ]
        },
        {
          "id": "516a32c0-da5f-408b-9f2a-d2037f1a079e",
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
              "id": "38fefff9-b480-4fdf-9ba2-d18ecc82efce"
            }
          ]
        },
        {
          "id": "5fcadaf7-761c-4323-beae-29633c72ca30",
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
              "id": "7f82a922-fadb-4791-a895-11b9a141b218"
            }
          ]
        }
      ]
    },
    {
      "name": "Listings",
      "item": [
        {
          "id": "ef4ea402-d757-4eb0-9d56-9993b55b4f19",
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
              "id": "84d888df-2c94-4a1e-a0cc-3772c1d7cf58"
            }
          ]
        },
        {
          "id": "1df29074-3c93-43cb-9709-f78ca43bdb4e",
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
              "id": "f1312d0a-8eb4-47c8-a1b5-678febb242e7"
            }
          ]
        },
        {
          "id": "daf26f44-4298-4a0a-b76a-9b0334cb9459",
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
              "id": "455ffbc2-5f1f-4145-b7ff-7e21ee9d4e59"
            }
          ]
        },
        {
          "id": "5a94fac4-c418-435d-abf8-2d37de688b72",
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
              "id": "809e8fa1-ea36-4027-a493-4589bed49fd6"
            }
          ]
        },
        {
          "id": "ad897566-74af-4334-b1e5-04e45eada685",
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
              "id": "602eefba-f13a-4f24-aa3b-f1a059030012"
            }
          ]
        },
        {
          "id": "a9f6c8e3-1af3-4a36-b18e-69ff6cec892c",
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
              "id": "71ff912b-94a5-42b6-a343-0dc862a7a6b6"
            }
          ]
        },
        {
          "id": "df69ed99-b97a-45c4-954b-c922ea59777e",
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
              "id": "d93edc27-c0ff-4122-8152-d3d8070cd9eb"
            }
          ]
        },
        {
          "id": "15101c54-1b29-45a1-bf13-02f816e74366",
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
              "id": "1eeb808d-520f-4752-bd8f-19f0eeb75921"
            }
          ]
        },
        {
          "id": "a61c10f1-9431-406f-97a2-88d93f4cea30",
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
              "id": "6bdd3053-2c22-4613-b5a0-1cb50cd5b09e"
            }
          ]
        },
        {
          "id": "b2b0133d-f176-43a3-8173-5c1862628c03",
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
              "id": "70498f8c-194c-4239-a035-f2dfa504c35e"
            }
          ]
        },
        {
          "id": "b062c2ad-a21d-4a52-8e18-afeacab95086",
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
              "id": "cd4d4b10-95ae-4aca-bd29-0bb0be8ae5e0"
            }
          ]
        },
        {
          "id": "4992cc9b-968a-44bd-bc41-90f655e7d88c",
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
              "id": "894d4257-cb1e-43bf-873c-66b308fce47d"
            }
          ]
        },
        {
          "id": "5c13a49b-fdb2-497c-ae51-dc4a07b83e09",
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
              "id": "e88893bb-6132-4b94-957b-32ceb086db11"
            }
          ]
        }
      ]
    },
    {
      "name": "Shops",
      "item": [
        {
          "id": "8fb405f1-a16a-487e-9e39-abbc02cb79a1",
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
              "id": "8fba56eb-82f5-4d8a-a6d6-ebcc102ddf71"
            }
          ]
        },
        {
          "id": "e51e2a16-835d-4193-b125-d5957b515705",
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
              "id": "8fcf8320-e8a6-4740-a38f-25a1521541c3"
            }
          ]
        },
        {
          "id": "61f9b5fe-60e6-45a3-94c8-ca23414369fd",
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
              "id": "be779757-30ea-4330-b1a5-f397883361a9"
            }
          ]
        },
        {
          "id": "ed27bd84-4d10-4e22-a49b-7a60954be078",
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
              "id": "b2a9017d-4806-4203-b826-350eec3e624e"
            }
          ]
        },
        {
          "id": "3bedf368-c55a-49a3-9031-a61e99b1e334",
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
              "id": "f150f7c1-d4c0-4afc-ab40-0c51b6ad3149"
            }
          ]
        },
        {
          "id": "1badf45e-4872-474a-8ff9-8afab614bda5",
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
              "id": "7b211bad-e147-4af8-8667-8eeca756086c"
            }
          ]
        },
        {
          "id": "baa5ea02-74c3-497f-a5b1-86cc2607f4bd",
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
              "id": "fc0cac77-f14f-4c54-92a9-ba06417e1155"
            }
          ]
        },
        {
          "id": "d97f1eb2-29ec-4866-a396-1e8854b91b0f",
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
              "id": "3908feb3-580c-486e-a1b3-1c298e42cc5f"
            }
          ]
        },
        {
          "id": "cda9aad9-6930-42f5-a7c2-c8a0158756ca",
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
              "id": "367aa614-4582-4b76-ae5d-7a081a2df507"
            }
          ]
        },
        {
          "id": "58c2fb7b-302f-4395-8ea0-c6762ba9e80e",
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
              "id": "323f7c5c-0e47-49c7-bf3f-6ef1c0fcc345"
            }
          ]
        },
        {
          "id": "7da77a5c-63ec-46f1-8a83-763e29084a07",
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
              "id": "9b896a10-0a50-43a0-b81b-6b835bb96689"
            }
          ]
        },
        {
          "id": "6a233afb-f930-4342-ab83-2499f1ff8f7c",
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
              "id": "15583ac5-5c08-474f-b33a-805b9aa1becc"
            }
          ]
        },
        {
          "id": "f218c28a-0364-44d0-9c36-7c5c29df4441",
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
              "id": "ebd0f710-42b1-4bd3-920c-0f3c86cbb073"
            }
          ]
        },
        {
          "id": "95df1302-1f64-49a4-81de-61371484bf71",
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
              "id": "e36a0827-4e60-45da-8ae3-d6115169721e"
            }
          ]
        }
      ]
    },
    {
      "name": "Orders",
      "item": [
        {
          "id": "f373ee9a-15fa-4c29-b934-a1d74841375d",
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
              "id": "b22b918c-455e-42d7-b3a8-8c57001535bd"
            }
          ]
        },
        {
          "id": "b8132e9f-19bd-4035-a49c-fa459fd4f69f",
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
              "id": "21ea3377-8f6f-4449-a853-3e6d266a8646"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipts",
      "item": [
        {
          "id": "976e291b-e826-4533-8155-e9a4bc62ccd0",
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
              "id": "e152dde3-f8c5-4df9-842f-bfe7c2a8ddfa"
            }
          ]
        },
        {
          "id": "fce43421-f1e0-42b6-adfa-c8de770f5f42",
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
              "id": "d1a4a4aa-7d91-485f-9a9c-829d270dfbe8"
            }
          ]
        },
        {
          "id": "0050ecc6-7a68-485e-a29a-cb779aec32b5",
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
              "id": "465a8b0f-c336-4d58-84b8-08a4c21ea621"
            }
          ]
        }
      ]
    },
    {
      "name": "Regions",
      "item": [
        {
          "id": "9b085b98-2200-4736-8c8f-3a6a6061fbbb",
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
              "id": "73e1379c-1140-4fdf-bfa4-7562fab5fa08"
            }
          ]
        },
        {
          "id": "21992cd5-7f1a-4779-a3a5-ab75a8139cee",
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
              "id": "58ad5fe5-89fb-4ee7-82fb-70d954e44833"
            }
          ]
        }
      ]
    },
    {
      "name": "Shipping",
      "item": [
        {
          "id": "6a3327eb-1013-4ce7-9baf-850cec05933b",
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
              "id": "c3c4fbb8-7630-4cde-b774-edb6f040dccc"
            }
          ]
        },
        {
          "id": "b53408b0-1bd1-4360-bedf-416df8c42e9d",
          "name": "putShippingInfoShippingInfo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
           