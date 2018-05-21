{
  "info": {
    "name": "Etsy Get",
    "_postman_id": "d3122a59-2e1e-445a-890a-e53fd83d2c4f",
    "description": "Get a list of all methods available.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "db1e6a7c-27bc-4ec2-8bf4-0aa0bd606775",
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
              "id": "ad3e37b3-479d-4ee6-ade9-eb217e98b991"
            }
          ]
        },
        {
          "id": "aad2ba44-29ca-41bb-95f8-44f6159e0efd",
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
              "id": "c2671800-5d70-42a9-8b6f-03a6b1a7e924"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "db97e766-52db-49f9-a840-71b4f032912c",
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
              "id": "198202c1-2d72-43c4-a309-e3b0201a731a"
            }
          ]
        },
        {
          "id": "2d3c4e65-5ae5-44d8-9d38-8c45bdabdb94",
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
              "id": "1ff4b1cb-376c-4abf-bcca-0469420e26b5"
            }
          ]
        },
        {
          "id": "3413eedb-9fe7-43b2-aeeb-7996a6221636",
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
              "id": "4ffc6088-96cb-4644-8623-7866d860dda1"
            }
          ]
        },
        {
          "id": "88ac19b7-4e85-4264-b374-e5afa9463256",
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
              "id": "3700b937-075d-4b26-bb6c-b07e2c80468f"
            }
          ]
        },
        {
          "id": "1960a031-8d7a-4883-8539-20e695396ba3",
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
              "id": "5e0afc7e-cfb1-4c27-8a02-c49d35eca370"
            }
          ]
        },
        {
          "id": "fc43ffa7-22c0-424a-9d45-d1ee400226f7",
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
              "id": "79ba9c0d-646f-421a-ac0f-b36b042ce29f"
            }
          ]
        },
        {
          "id": "d08a7e08-44a2-40d7-a14d-7504d96056b5",
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
              "id": "46dad334-2569-4c7e-98f9-14241c02d8aa"
            }
          ]
        },
        {
          "id": "055b3c6d-5eb3-447f-b6ac-b1bf503b1eda",
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
              "id": "76c36381-4553-4da6-b5a2-21e36a912fe7"
            }
          ]
        },
        {
          "id": "31161159-a0b1-47d5-80ea-5dfae8f36d30",
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
              "id": "5be22867-f2b0-409f-89f3-26c7474ab3ba"
            }
          ]
        },
        {
          "id": "fac92bfd-ee35-4f1d-92e4-95ec68da5293",
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
              "id": "f9c467a5-1fe8-44d8-81bf-651981f6b9b7"
            }
          ]
        },
        {
          "id": "4687d766-66e7-4cd8-8cfa-f1e00f58b2b6",
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
              "id": "705e8bf7-ddb4-450d-a256-de26da66c6b7"
            }
          ]
        },
        {
          "id": "f6535660-a3d2-49f8-9ff0-76220a8574b3",
          "name": "getUsersUserTreasuries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/treasuries"
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
            "description": "Get a user's Treasuries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29760cdf-050b-45c0-8188-5d699d1b3fd4"
            }
          ]
        },
        {
          "id": "2e9f3a76-d681-4fae-8157-4cab1769106d",
          "name": "getUsersUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id"
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
            "description": "Retrieves a User by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4f505bb-5289-484f-8f89-dc74c022eb7f"
            }
          ]
        },
        {
          "id": "04887ae3-a296-423f-abff-c6086899f794",
          "name": "getUsersUserShops",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/shops"
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
            "description": "Retrieves a set of Shop objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0c807c0-73d7-4869-a6eb-04228a5ff981"
            }
          ]
        },
        {
          "id": "1ae528cc-d488-4eb7-bb6c-a8e145618728",
          "name": "getUsersUserFavoredBy",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favored-by"
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
            "description": "Retrieves a set of FavoriteUser objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62618ea5-0f8a-4135-b3c2-f900a7ca5349"
            }
          ]
        },
        {
          "id": "8ed51353-ecac-4472-ac09-dec40427538a",
          "name": "getUsersUserFeedbackAsSubject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/feedback/as-subject"
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
            "description": "Retrieves a set of Feedback objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d96764d8-6a21-4089-a5cf-e79d59f9bc0f"
            }
          ]
        },
        {
          "id": "d332c065-fd4c-436f-879c-ce2519b2cb86",
          "name": "getUsersUserFeedbackAsAuthor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/feedback/as-author"
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
            "description": "Retrieves a set of Feedback objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "faa79be0-ba1a-4330-8ea3-124d4ee24411"
            }
          ]
        },
        {
          "id": "7c4174bf-c67e-439c-813d-cc425c0fdbbd",
          "name": "getUsersUserFeedbackAsBuyer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/feedback/as-buyer"
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
            "description": "Retrieves a set of Feedback objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c107622b-47f6-4213-ae49-cbfaf0c64860"
            }
          ]
        },
        {
          "id": "8c865be4-d07f-4110-9f3a-3471c1e9acc8",
          "name": "getUsersUserFeedbackAsSeller",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/feedback/as-seller"
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
            "description": "Retrieves a set of Feedback objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d4a81f2-fda8-4176-8af5-e4d2c2494408"
            }
          ]
        },
        {
          "id": "e38b582f-d17d-4c85-9fd4-3a289c6f6a38",
          "name": "getUsersUserOrders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/orders"
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
            "description": "Retrieves a set of Order objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ad96e07-22d9-4585-a70c-aaa6cc7e031c"
            }
          ]
        },
        {
          "id": "403e9414-0c6e-4e5d-a225-aef59af8a3c9",
          "name": "getUsersUserReceipts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/receipts"
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
            "description": "Retrieves a set of Receipt objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd8f2d3b-9334-49f2-ab04-250b9533b788"
            }
          ]
        },
        {
          "id": "54632e54-28d8-44b7-b8a1-29d65f1b41e4",
          "name": "getUsersUserTransactions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/transactions"
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
            "description": "Retrieves a set of Transaction objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6583ad21-836f-4661-a8a7-cf87a1613bdc"
            }
          ]
        },
        {
          "id": "78c89eeb-bd40-426f-bbb4-63351f49d6ed",
          "name": "getUsersUserCharges",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/charges"
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
            "description": "Retrieves a set of BillCharge objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d4891b2-0dd3-4d07-a743-349b1acf14ff"
            }
          ]
        },
        {
          "id": "d629e9c5-87dd-46e9-a03e-e094b3efb96b",
          "name": "getUsersUserPayments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/payments"
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
            "description": "Retrieves a set of BillPayment objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa4785e8-9369-46de-a334-51cb680b9d6b"
            }
          ]
        },
        {
          "id": "d9a4b082-3ddd-4540-8928-697f92c6ac1d",
          "name": "getUsersUserShippingTemplates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/shipping/templates"
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
            "description": "Retrieves a set of ShippingTemplate objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c77f548-25a3-4cc5-a78f-28172fd3b531"
            }
          ]
        },
        {
          "id": "27f107bf-63b6-4613-a73d-af1e6e87e9a4",
          "name": "getUsersUserPaymentsTemplates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/payments/templates"
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
            "description": "Retrieves a set of PaymentTemplate objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5baf504-3501-44f4-a73a-7354fbb5f309"
            }
          ]
        },
        {
          "id": "de1c02bf-c4fd-4810-8cd0-e05904ef52ec",
          "name": "getUsersUserAddresses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/addresses"
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
            "description": "Retrieves a set of UserAddress objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cd8a488-346c-49d3-a884-8bb6db866183"
            }
          ]
        },
        {
          "id": "cc8c8fb7-6647-4d36-9d2a-65f68be51643",
          "name": "postUsersUserAddresses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/addresses"
              ],
              "query": [
                {
                  "key": "city",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "country_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "first_line",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "second_line",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "zip",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new UserAddress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ea206ea-2413-478e-a16e-451bc72b1bea"
            }
          ]
        },
        {
          "id": "c90ca084-a9bf-48f6-9cf2-fded9fcc2a70",
          "name": "postUsersUserAvatar",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/avatar"
              ],
              "query": [
                {
                  "key": "image",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "src",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload a new user avatar image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5945f2a6-9857-49af-8e7f-f8d335a1e639"
            }
          ]
        },
        {
          "id": "8dc5296e-13f2-4ad2-9cb4-859b6a3d5ead",
          "name": "getUsersUserAvatarSrc",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/avatar/src"
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
            "description": "Get avatar image source"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1017c17-5698-4383-8ff2-73e2ec3bc6f8"
            }
          ]
        },
        {
          "id": "bb6c0d59-d1c2-469d-a20d-88f4284796c2",
          "name": "getUsersUserAddressesUserAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/addresses/:user_address_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "user_address_id",
                  "value": "user_address_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a UserAddress by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "adb524b1-f017-4381-8994-68cb60fa5a5b"
            }
          ]
        },
        {
          "id": "f9f60929-1824-4887-807a-4f8e15fdc46e",
          "name": "putUsersUserAddressesUserAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/addresses/:user_address_id"
              ],
              "query": [
                {
                  "key": "city",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "country_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "first_line",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "second_line",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "zip",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "user_address_id",
                  "value": "user_address_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a UserAddress with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a39457b1-c658-4920-b3e9-34def9911ebe"
            }
          ]
        },
        {
          "id": "ddcc5b1d-3952-43b4-8e51-32344ae24bec",
          "name": "deleteUsersUserAddressesUserAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/addresses/:user_address_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "user_address_id",
                  "value": "user_address_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the UserAddress with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28ca7156-9a86-48eb-a1e8-43a5749c55bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Home Pages",
      "item": [
        {
          "id": "14d914f2-299a-48dc-b840-291dec0645ad",
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
              "id": "a29a2dad-7d30-4c11-b2ec-41f059e56dca"
            }
          ]
        },
        {
          "id": "a06d3312-ba14-42d6-82b9-2aa5c02e04ad",
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
              "id": "3cd8175c-4f9b-4590-9e10-0841067e5a7f"
            }
          ]
        },
        {
          "id": "d7f34902-e926-4380-8d19-9db9ab75d94a",
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
              "id": "908486a7-7535-4280-a9b0-6349764f19e9"
            }
          ]
        },
        {
          "id": "df8ba7e3-2d39-4f4e-bd36-91cad5e0a48d",
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
              "id": "5dced38f-b305-4248-9752-4b37b045df2b"
            }
          ]
        },
        {
          "id": "c69ed39f-7440-4111-8cfa-5bfef1560550",
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
              "id": "de82ad2e-4f4d-441e-9a4b-be66e0671057"
            }
          ]
        },
        {
          "id": "7abd3061-a026-4938-be84-7ce174828b39",
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
              "id": "641f32e5-a50f-40a0-9354-49735bac1211"
            }
          ]
        },
        {
          "id": "63a26ed3-f821-4f43-bd5d-70f6d6ba2e55",
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
              "id": "d8f9d926-2bd9-4469-814c-840568ee2e36"
            }
          ]
        },
        {
          "id": "11db15f4-7d65-46f7-b604-7ea5abffb5cc",
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
              "id": "beab4fe8-a20b-4262-a0e3-f939e2b882e5"
            }
          ]
        },
        {
          "id": "ee979311-956a-4f4e-9495-1415aa0105ce",
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
              "id": "cebab428-9767-4940-9ba0-64a6fa5e18bc"
            }
          ]
        },
        {
          "id": "1f23829d-c6ab-42b4-943f-ba3235fdf1b2",
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
              "id": "a77b86a2-0f66-48c2-b194-f3b042838025"
            }
          ]
        }
      ]
    },
    {
      "name": "Listings",
      "item": [
        {
          "id": "ee05bcd3-2898-4a37-866a-b6f96e2fcff5",
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
              "id": "3c9cef65-32a1-4a46-9efa-a230de9e0734"
            }
          ]
        },
        {
          "id": "fd9753c4-c5f3-4aa7-8b02-d09e609a96f9",
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
              "id": "18da88b2-4ba1-42bd-a9c8-f44b1510c03b"
            }
          ]
        },
        {
          "id": "c022d486-41d8-453e-a693-17b004d05f5a",
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
              "id": "2351b108-5de6-4719-bb23-81b5eb281541"
            }
          ]
        },
        {
          "id": "5e0520c9-a002-4d05-9ae1-6d7e8585fdfc",
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
              "id": "d797c8bb-c7eb-44b4-8f5e-faba01c882f7"
            }
          ]
        },
        {
          "id": "2907cb0c-4042-4735-aabc-3edfc049f0e9",
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
              "id": "016e50b8-3054-4c92-827e-46f677b84fcc"
            }
          ]
        },
        {
          "id": "c1fc4b0d-6704-4962-8df8-05d6f2575d8d",
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
              "id": "89eb215f-e347-47fe-a5cf-801f2ef1cce7"
            }
          ]
        },
        {
          "id": "0e803cc0-19fd-4729-8efe-4180d68fe243",
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
              "id": "85657a2a-76f4-4ad9-889a-1a8e43171c2e"
            }
          ]
        },
        {
          "id": "01f1a1ed-d547-4145-a5ff-983ba445de11",
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
              "id": "897f53fa-5df4-4c4c-87cd-3ebfa581c167"
            }
          ]
        },
        {
          "id": "d1cd0774-fd56-4fef-8150-859831b301d1",
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
              "id": "acb005c3-dc34-4efe-ba69-664f3c8b4bc7"
            }
          ]
        },
        {
          "id": "c6330c12-5183-48dd-852a-c3837fd6e862",
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
              "id": "5d8147a5-b9a7-43ca-ba2b-31da53b88fac"
            }
          ]
        },
        {
          "id": "1137163f-525c-4c17-ac89-d8da38d7bdf1",
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
              "id": "1f7025ed-4a58-429c-96a1-7b0b5d9af526"
            }
          ]
        },
        {
          "id": "fb119bfb-77c9-4546-ac3c-8877833a5f7d",
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
              "id": "90645844-0a03-4fdf-b354-5333b26282c6"
            }
          ]
        },
        {
          "id": "8af65a1c-2532-43b2-94a2-504aa0734a35",
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
              "id": "52319dec-89ab-4990-a43f-7d2ac913a53e"
            }
          ]
        }
      ]
    },
    {
      "name": "Shops",
      "item": [
        {
          "id": "0de64418-d2e1-4793-8b05-1e1f5b390a58",
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
              "id": "833ffc7d-4a1d-4769-b1ec-4806b5c1ab6f"
            }
          ]
        },
        {
          "id": "e0df8b05-98c1-4115-9ed5-1aac41ac1df2",
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
              "id": "70e784ff-4019-42e6-8e54-c08678f7e5d8"
            }
          ]
        },
        {
          "id": "992c45cb-7f03-4f17-81b2-dedca6e38219",
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
              "id": "eeb91a14-f82f-4be3-91fa-dcea3f93fdd1"
            }
          ]
        },
        {
          "id": "ae67eb7f-fe1f-47ce-ac41-f287a62bec58",
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
              "id": "fc003325-9116-4e8f-90a1-9634760bc8ad"
            }
          ]
        },
        {
          "id": "b546cb46-fe0b-4498-8650-ee16d341ce40",
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
              "id": "069e2348-271b-444a-b3b9-1d2ebd2989c8"
            }
          ]
        },
        {
          "id": "fde1dd8c-fc9f-4c28-9f1f-4c1e35f2af35",
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
              "id": "058919f9-d7bb-48b6-b645-03548935560a"
            }
          ]
        },
        {
          "id": "33077c3e-af2c-4d3d-8783-a5197c1f8535",
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
              "id": "a6e8fd70-f6b8-462e-ba95-797f7a710aca"
            }
          ]
        },
        {
          "id": "b477abbb-ccac-490e-8d96-3dc28e129adf",
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
              "id": "fcff0951-a1c6-4da0-8924-56a73d232a7f"
            }
          ]
        },
        {
          "id": "fe38a6c3-5e73-4f64-8130-d5e896365f1f",
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
              "id": "ee57300b-ba3e-42d4-a740-ac6add448bc0"
            }
          ]
        },
        {
          "id": "2af8156c-f9ba-4bf1-8050-89c54438a602",
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
              "id": "48f2b26c-c66b-4fb4-b871-0d67fef35707"
            }
          ]
        },
        {
          "id": "62a5e4b5-d770-43b3-8de2-38f6543fab26",
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
              "id": "a6a004bf-fc48-472d-aa7b-ddbcb5b8b2af"
            }
          ]
        },
        {
          "id": "ecc99178-6da3-46a9-96cc-f269fa7a3c09",
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
              "id": "9644163e-9b1b-4f50-9705-5965d6bb0384"
            }
          ]
        },
        {
          "id": "02694e0a-eaa5-44d6-87d6-096c5c812d2c",
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
              "id": "6795ea93-5e9c-4e85-89cc-ba111904ad90"
            }
          ]
        },
        {
          "id": "26d3ce66-f00d-4e02-b13b-8e321cc81757",
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
              "id": "01f52659-70d7-42a6-96cc-623ced913934"
            }
          ]
        }
      ]
    },
    {
      "name": "Orders",
      "item": [
        {
          "id": "9647d8a4-a036-4c5c-b488-d0989d9e05ae",
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
              "id": "964fe5e1-dc35-468d-be89-84db172f3d22"
            }
          ]
        },
        {
          "id": "51b52193-a52d-4c2d-967e-ea1e58aa9b3f",
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
              "id": "1f4ceb81-d236-43d8-ac95-575790190127"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipts",
      "item": [
        {
          "id": "874d0a63-5920-45b5-9580-b1c2567dcaeb",
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
              "id": "65dcb670-79ed-4176-a499-e0c13dd809fb"
            }
          ]
        },
        {
          "id": "2aa1799a-549e-420a-bb8c-5c957638413a",
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
              "id": "b550d307-78ef-4142-b5bd-72c9c1bbddb9"
            }
          ]
        },
        {
          "id": "4dfaa04b-0a61-4102-9dac-4e29267ff983",
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
              "id": "d07f3fdd-7ceb-4a46-a565-2d47fa0410f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Regions",
      "item": [
        {
          "id": "3967d4f6-02b2-4b47-bbe7-e63b0b709ad3",
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
              "id": "8dd04db6-e20d-4c67-9f80-b46b39837a1e"
            }
          ]
        },
        {
          "id": "7728b23f-fcc5-44c8-9c6a-95e6362105a8",
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
              "id": "178bc567-a430-48ec-9ae8-dfa3fe4fdb0b"
            }
          ]
        }
      ]
    },
    {
      "name": "Shipping",
      "item": [
        {
          "id": "fe6a79e7-7b30-4556-8cce-78472f13cbad",
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
              "id": "5643b6dd-c078-4c8d-9300-fb14243628ed"
            }
          ]
        },
        {
          "id": "2cdb7b5e-4aa7-40bc-99d0-04201f514ea5",
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
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a ShippingInfo with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "622ca586-ad4b-4a5e-ab53-e05cdeb8bd2d"
            }
          ]
        },
        {
          "id": "dbb3a07f-9637-458d-9046-cc1a3376f715",
          "name": "deleteShippingInfoShippingInfo",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the ShippingInfo with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "726bc436-a13e-40f1-95e7-0572756ad042"
            }
          ]
        },
        {
          "id": "23977ed8-e0ea-4338-bcbd-a05d2b9dea12",
          "name": "getShippingTemplatesEntriesShippingTemplateEntry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shipping/templates/entries/:shipping_template_entry_id"
              ],
              "variable": [
                {
                  "id": "shipping_template_entry_id",
                  "value": "shipping_template_entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a ShippingTemplateEntry by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c690a15a-dbd4-4e19-a6a3-0e9cbd1c1660"
            }
          ]
        },
        {
          "id": "e26d6a40-2f6f-4036-aef3-b8092cfb5773",
          "name": "putShippingTemplatesEntriesShippingTemplateEntry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shipping/templates/entries/:shipping_template_entry_id"
              ],
              "query": [
                {
                  "key": "destination_country_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "primary_cost",
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
                  "id": "shipping_template_entry_id",
                  "value": "shipping_template_entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a ShippingTemplateEntry"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76bc4ea3-aff4-479a-a38c-7f81084a56b6"
            }
          ]
        },
        {
          "id": "71a06ba8-699c-4115-a233-5adb7fee4939",
          "name": "deleteShippingTemplatesEntriesShippingTemplateEntry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shipping/templates/entries/:shipping_template_entry_id"
              ],
              "variable": [
                {
                  "id": "shipping_template_entry_id",
                  "value": "shipping_template_entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a ShippingTemplateEntry"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11bd32cc-5c37-4fe8-a8ac-f74f36b33d5e"
            }
          ]
        },
        {
          "id": "8452811d-25e4-4f34-9924-3eb08196de14",
          "name": "postShippingTemplatesEntries",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/shipping/templates/entries?destination_country_id=%7B%7D&destination_region_id=%7B%7D&primary_cost=%7B%7D&secondary_cost=%7B%7D&shipping_template_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new ShippingTemplateEntry"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4dc83007-eb76-4fef-9924-dad57c6d1dc5"
            }
          ]
        },
        {
          "id": "d63b21ac-6d77-4e1d-ad95-c9db4d74bc63",
          "name": "getShippingTemplatesShippingTemplate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shipping/templates/:shipping_template_id"
              ],
              "variable": [
                {
                  "id": "shipping_template_id",
                  "value": "shipping_template_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a ShippingTemplate by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6bc42ea-63c8-4614-b3db-86fba54a2713"
            }
          ]
        },
        {
          "id": "2ec5762e-c4ae-4624-8611-88bc37738e8c",
          "name": "putShippingTemplatesShippingTemplate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shipping/templates/:shipping_template_id"
              ],
              "query": [
                {
                  "key": "origin_country_id",
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
                  "id": "shipping_template_id",
                  "value": "shipping_template_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a ShippingTemplate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c51f111-b1e3-46a2-8f1f-51d4118af437"
            }
          ]
        },
        {
          "id": "bf934b77-3129-4e65-87d5-0adc953f2b13",
          "name": "deleteShippingTemplatesShippingTemplate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shipping/templates/:shipping_template_id"
              ],
              "variable": [
                {
                  "id": "shipping_template_id",
                  "value": "shipping_template_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the ShippingTemplate with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93fc18aa-6fb6-4372-9b9a-b946a5f6e122"
            }
          ]
        },
        {
          "id": "86ca934e-f9b3-4872-8bd7-43e739be3770",
          "name": "getShippingTemplatesShippingTemplateEntries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shipping/templates/:shipping_template_id/entries"
              ],
              "variable": [
                {
                  "id": "shipping_template_id",
                  "value": "shipping_template_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of ShippingTemplateEntry objects associated to a ShippingTemplate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df62ccdf-3618-430a-a93b-e0e8aee32628"
            }
          ]
        },
        {
          "id": "f9fd4953-bec0-4206-a2ee-2ecdf919df6b",
          "name": "postShippingTemplates",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/shipping/templates?destination_country_id=%7B%7D&destination_region_id=%7B%7D&origin_country_id=%7B%7D&primary_cost=%7B%7D&secondary_cost=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new ShippingTemplate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2a488a6-eaf4-4a22-8c1b-1d82a83f85dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Sections",
      "item": [
        {
          "id": "e7a5a0c7-95d7-43de-9219-a4e6ad84a0d4",
          "name": "getSectionsShopSection",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "sections/:shop_section_id"
              ],
              "variable": [
                {
                  "id": "shop_section_id",
                  "value": "shop_section_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a ShopSection by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e3c5a38-35c0-4231-89e5-8161a98976bb"
            }
          ]
        },
        {
          "id": "4c522550-ee8d-44ca-99c4-a6f8918c2a7f",
          "name": "putSectionsShopSection",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "sections/:shop_section_id"
              ],
              "query": [
                {
                  "key": "rank",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "shop_section_id",
                  "value": "shop_section_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a ShopSection with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df5e809f-59c7-4762-ba03-421df4bcf040"
            }
          ]
        },
        {
          "id": "b608d5c8-685e-4ab6-a22a-3f1b8a356085",
          "name": "deleteSectionsShopSection",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "sections/:shop_section_id"
              ],
              "variable": [
                {
                  "id": "shop_section_id",
                  "value": "shop_section_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the ShopSection with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b132e9e9-ab05-4bb0-83c5-6845d574ec1f"
            }
          ]
        },
        {
          "id": "e12ed4b9-1619-4e6d-8fec-0e096d0c1f6a",
          "name": "postSections",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/sections?title=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new ShopSection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af9af72b-ba32-4b40-800f-9e02338934da"
            }
          ]
        }
      ]
    },
    {
      "name": "Categories",
      "item": [
        {
          "id": "7feed56b-ae89-4002-8b54-d72c43d6a756",
          "name": "getCategoriesTag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "categories/:tag"
              ],
              "variable": [
                {
                  "id": "tag",
                  "value": "tag",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a top-level Category by tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2675b8fc-799b-407b-80cd-b77d2edf2b56"
            }
          ]
        },
        {
          "id": "359fdd2c-aa10-44d4-a11a-8b7637d24612",
          "name": "getCategoriesTagSubtag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "categories/:tag/:subtag"
              ],
              "variable": [
                {
                  "id": "tag",
                  "value": "tag",
                  "type": "string"
                },
                {
                  "id": "subtag",
                  "value": "subtag",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a second-level Category by tag and subtag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14cab21d-b9ab-4828-a5d8-08617c058bf2"
            }
          ]
        },
        {
          "id": "3d4e3253-5a8a-4811-9d26-160a15e0a324",
          "name": "getCategoriesTagSubtagSubsubtag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "categories/:tag/:subtag/:subsubtag"
              ],
              "variable": [
                {
                  "id": "tag",
                  "value": "tag",
                  "type": "string"
                },
                {
                  "id": "subtag",
                  "value": "subtag",
                  "type": "string"
                },
                {
                  "id": "subsubtag",
                  "value": "subsubtag",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a third-level Category by tag, subtag and subsubtag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31b38bfd-209c-4360-95a2-29e3c385e535"
            }
          ]
        }
      ]
    },
    {
      "name": "Taxonomy",
      "item": [
        {
          "id": "8a7579b8-c98b-4640-a400-763888292547",
          "name": "getTaxonomyCategories",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/taxonomy/categories",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all top-level Categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89ea67bb-6fe0-43bb-91e1-7f1300cc56a8"
            }
          ]
        },
        {
          "id": "9493ca4d-8326-4218-aad8-98d347a3f309",
          "name": "getTaxonomyCategoriesTag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "taxonomy/categories/:tag"
              ],
              "variable": [
                {
                  "id": "tag",
                  "value": "tag",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves children of a top-level Category by tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0554b802-a1fd-4556-b5fc-782fdda78c6e"
            }
          ]
        },
        {
          "id": "e3b797e6-e2a0-4b0f-b3c5-6526f3d0f59e",
          "name": "getTaxonomyCategoriesTagSubtag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "taxonomy/categories/:tag/:subtag"
              ],
              "variable": [
                {
                  "id": "tag",
                  "value": "tag",
                  "type": "string"
                },
                {
                  "id": "subtag",
                  "value": "subtag",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves children of a second-level Category by tag and subtag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37a2eab9-db98-44f8-85c1-9cab5c9f55fa"
            }
          ]
        },
        {
          "id": "d3a7493b-d5c5-425f-9ce6-8b85b0a04334",
          "name": "getTaxonomyTags",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/taxonomy/tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all related tags for the given tag set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f534e2f7-f27a-4cc9-9553-f28caf5383a2"
            }
          ]
        },
        {
          "id": "f0bface5-398b-49e1-9054-19b0fff451bb",
          "name": "getTaxonomyTagsTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "taxonomy/tags/:tags"
              ],
              "variable": [
                {
                  "id": "tags",
                  "value": "tags",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all related tags for the given tag set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa250b5d-004f-455e-82e8-c8431a344401"
            }
          ]
        }
      ]
    },
    {
      "name": "Transactions",
      "item": [
        {
          "id": "3286e40e-5cea-42e9-aa24-bb76d7af2037",
          "name": "getTransactionsTransaction",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "transactions/:transaction_id"
              ],
              "variable": [
                {
                  "id": "transaction_id",
                  "value": "transaction_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Transaction by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa060f18-73dd-4d01-903d-f59d96303e9e"
            }
          ]
        }
      ]
    },
    {
      "name": "Treasuries",
      "item": [
        {
          "id": "6d8383c4-ae3f-4d69-9032-70feba5e6cef",
          "name": "getTreasuriesTreasury",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "treasuries/:treasury_id"
              ],
              "variable": [
                {
                  "id": "treasury_id",
                  "value": "treasury_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a Treasury"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "903c017c-f6be-4758-8d64-fb7820e1c2bf"
            }
          ]
        },
        {
          "id": "80fc4d21-e7c0-4ed6-ab67-86eadce998a5",
          "name": "getTreasuries",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/treasuries",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search Treasuries or else List all Treasuries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f569da7a-a08c-4315-85cb-fcda41664d0a"
            }
          ]
        }
      ]
    },
    {
      "name": "Payments",
      "item": [
        {
          "id": "4803a112-acba-44ce-b705-2ff6bcf4fc02",
          "name": "getPaymentsTemplatesPaymentTemplate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "payments/templates/:payment_template_id"
              ],
              "variable": [
                {
                  "id": "payment_template_id",
                  "value": "payment_template_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a PaymentTemplate by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd8d7829-8f90-492f-8bd5-d31b5e11245d"
            }
          ]
        },
        {
          "id": "bb825aba-10ae-490b-83c8-4cf428bacc7c",
          "name": "putPaymentsTemplatesPaymentTemplate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "payments/templates/:payment_template_id"
              ],
              "query": [
                {
                  "key": "allow_check",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "allow_mo",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "allow_other",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "allow_paypal",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "city",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "country_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "first_line",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "paypal_email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "second_line",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "zip",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "payment_template_id",
                  "value": "payment_template_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a PaymentTemplate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3f9065d-b2a3-4a80-b7d5-e1f90d940d46"
            }
          ]
        },
        {
          "id": "943bde46-7775-43cb-a248-c53e3ff76b11",
          "name": "postPaymentsTemplates",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/payments/templates?allow_check=%7B%7D&allow_mo=%7B%7D&allow_other=%7B%7D&allow_paypal=%7B%7D&city=%7B%7D&country_id=%7B%7D&first_line=%7B%7D&name=%7B%7D&paypal_email=%7B%7D&second_line=%7B%7D&state=%7B%7D&zip=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new PaymentTemplate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ce86375-a396-4465-ba36-da92976c1b5d"
            }
          ]
        },
        {
          "id": "01a1abc9-dbcd-4eac-93c9-be4c947bbcff",
          "name": "getPaymentsListingPayment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "payments/:listing_payment_id"
              ],
              "variable": [
                {
                  "id": "listing_payment_id",
                  "value": "listing_payment_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a ListingPayment by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18619080-ee29-4ab3-b84e-58581f15e37e"
            }
          ]
        }
      ]
    },
    {
      "name": "Featured",
      "item": [
        {
          "id": "4bdfa3c7-e7ef-4c57-9592-a3e4fa28e5fa",
          "name": "getFeaturedUsers",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/featured/users",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all FeaturedUser."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8189dce4-559a-4fb5-9a40-d5d45885d2e1"
            }
          ]
        },
        {
          "id": "f74e0396-a8db-4431-a953-d3c1b1df71a6",
          "name": "getFeaturedUsersFeaturedUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "featured/users/:featured_user_id"
              ],
              "variable": [
                {
                  "id": "featured_user_id",
                  "value": "featured_user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a FeaturedUser by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88d75dfc-b786-41bd-9ac0-5a68faac288e"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "c15baa29-efb8-4fa5-a202-cec8eed1af85",
          "name": "get",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of all methods available."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ff986f7-f4a0-4e84-b0b4-a66145d0017c"
            }
          ]
        }
      ]
    }
  ]
}