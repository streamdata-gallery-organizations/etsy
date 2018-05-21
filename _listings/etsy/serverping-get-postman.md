{
  "info": {
    "name": "Etsy Get Server Ping",
    "_postman_id": "1a28ca01-6a1f-443d-9fb8-3d5d57a559e8",
    "description": "Check that the server is alive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "f7585495-61bf-4aca-bf8e-5df38a2e8b3f",
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
              "id": "857f7624-7153-475d-89fb-31169d4aa5ef"
            }
          ]
        },
        {
          "id": "f881d39e-0959-4d2a-a0fb-6946827b1821",
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
              "id": "72b06f68-b246-478c-8326-5d6db8809ce8"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "d240979d-5517-4016-958b-b529dd151bd4",
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
              "id": "50f952a7-55b6-4a27-8e7b-d7c206cddeac"
            }
          ]
        },
        {
          "id": "6a082533-f436-451a-8b54-e46d5d03a454",
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
              "id": "5dd10b58-b91b-438a-9061-3983bb61ddcd"
            }
          ]
        },
        {
          "id": "1f83f938-9ba8-4db8-a4f6-78629fbf2450",
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
              "id": "673b341b-c2bc-4a4a-b297-94fb90cf96fd"
            }
          ]
        },
        {
          "id": "4090af1c-b8c7-41a6-9246-568caad2d784",
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
              "id": "f865179d-caa1-40cc-8e96-c8f80ede4c31"
            }
          ]
        },
        {
          "id": "0750eacd-0242-4195-96e2-61c22f5ab891",
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
              "id": "0c7da0d3-4d3f-4bae-ad84-daa62d95b54b"
            }
          ]
        },
        {
          "id": "3400916e-1a1a-4a22-950b-4eb070b8c148",
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
              "id": "78ae3ec1-d07c-417a-9f9d-00ad9a4dbf4e"
            }
          ]
        },
        {
          "id": "c881f3f3-9020-4cf7-bf24-04de485732ce",
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
              "id": "9e842a0a-6a1a-4b56-b589-905cbd8a6902"
            }
          ]
        },
        {
          "id": "cfc1832a-9874-46f3-a5b8-164734c26aed",
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
              "id": "2ba02fdd-2dbd-407f-85ff-3ff81dabd625"
            }
          ]
        },
        {
          "id": "0ad874d9-3518-4ad3-9993-7db68fc11a03",
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
              "id": "3a0049d2-2e9b-4c12-8009-0fbc51179961"
            }
          ]
        },
        {
          "id": "c59612d8-1855-4ae9-8c5b-f46cf2226f81",
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
              "id": "97938b1b-edb1-4674-a124-baf0a1621c52"
            }
          ]
        },
        {
          "id": "ffe2a722-56b1-4950-9ddb-49bab03de3b0",
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
              "id": "893c9254-14ea-465a-97ff-fd6d1d4ac91c"
            }
          ]
        },
        {
          "id": "88a99c0c-93f1-454c-b940-ad80a837defe",
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
              "id": "67ea9389-3039-4ece-bc7c-f627d7fc1bb4"
            }
          ]
        },
        {
          "id": "02ee5ab7-2748-4215-8025-db464e3494d1",
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
              "id": "9f61d2e1-85fc-437b-b333-831a30288193"
            }
          ]
        },
        {
          "id": "64bb520e-d814-4b9a-96ac-3c9d80a43628",
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
              "id": "1268f07d-cad2-486b-b695-2eba5c148883"
            }
          ]
        },
        {
          "id": "acc3b8f2-2983-4892-bfdf-1e5bbcaf2ae0",
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
              "id": "3487f2df-1a07-4940-80c5-501f192e75ca"
            }
          ]
        },
        {
          "id": "401d52b6-dc72-4528-ae70-c81a84c76788",
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
              "id": "fcde5077-c4a0-4e4b-80f2-da4bf417acf3"
            }
          ]
        },
        {
          "id": "0958aee0-4a4b-4437-9152-b020a486482e",
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
              "id": "659dd5ff-adff-424d-98ea-9942e323564b"
            }
          ]
        },
        {
          "id": "99337e5e-7fbe-45eb-935b-f5057753cd1e",
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
              "id": "46478e6c-ea37-4fa7-b151-3e0ef4b2dc8c"
            }
          ]
        },
        {
          "id": "e022fbe9-ded6-465c-abc7-19465274d6a2",
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
              "id": "ef10ee10-4376-4700-8a91-c06dbba96eb9"
            }
          ]
        },
        {
          "id": "a7ce9a57-1865-4c6b-b536-6ffd04a403fe",
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
              "id": "0ce98ad3-8df2-4348-944d-8f6176b82206"
            }
          ]
        },
        {
          "id": "b3b5250b-234f-4088-a7b8-91dc123ae768",
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
              "id": "7bde0687-d800-4939-876f-5dbe30119e2f"
            }
          ]
        },
        {
          "id": "cd060d1b-4a57-41d2-b654-fef0e4e73647",
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
              "id": "745d6487-b73c-4844-b842-333be8501e98"
            }
          ]
        },
        {
          "id": "fcd0c0f4-f1df-49a5-9b89-7dc6083ba92a",
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
              "id": "d8b53f14-1e25-4fc5-922e-4b05526d48a7"
            }
          ]
        },
        {
          "id": "76ee4250-5774-447c-8cc7-2bbecd5bc47c",
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
              "id": "d54b2f04-4267-4a70-acc1-75f24dffbe99"
            }
          ]
        },
        {
          "id": "59953076-e50c-4dbb-863a-1ddeebacbdfc",
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
              "id": "dbb4b3ec-d074-44c5-94fc-84e557790dbd"
            }
          ]
        },
        {
          "id": "11c45a3f-cba2-4137-b73c-007c0d86b26b",
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
              "id": "377efc3d-b85a-4ac9-b8c9-812f561bc376"
            }
          ]
        },
        {
          "id": "f203e858-0c7b-4770-8d48-87d04f2bca7c",
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
              "id": "fb6f2d40-79cf-43a1-9403-261753ca89af"
            }
          ]
        },
        {
          "id": "68bbd110-1767-4781-991b-346f55f8b287",
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
              "id": "82110150-7a2c-4ed8-84ca-aa92368c19cc"
            }
          ]
        },
        {
          "id": "05b72264-7ecf-4761-9afa-708fed02622b",
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
              "id": "dd4aee79-9d24-424d-adcd-317f90b4e76d"
            }
          ]
        },
        {
          "id": "c42dc941-1503-4f1d-8e48-e21b800390c7",
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
              "id": "d8617096-28f3-4af9-9078-7fee8b76535e"
            }
          ]
        },
        {
          "id": "90e176f0-bb61-4e48-892b-353fb97bc086",
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
              "id": "939b63f9-8960-467f-b7c1-ea14775e33c0"
            }
          ]
        },
        {
          "id": "61d10e84-8b8a-47d9-af56-35913f175baa",
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
              "id": "42a47dba-acd8-4a5e-8974-7337ba10e820"
            }
          ]
        },
        {
          "id": "32236a47-31e8-48f9-a266-ca9b5eee8bb1",
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
              "id": "fbb7e9c0-8379-440a-bbc3-1e5c3b6f605c"
            }
          ]
        }
      ]
    },
    {
      "name": "Home Pages",
      "item": [
        {
          "id": "48178f78-6c49-4055-9348-9cb32bb30b60",
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
              "id": "b2d74bfb-8fe1-446d-a335-64bf0e99d1e1"
            }
          ]
        },
        {
          "id": "3d3819bb-75a4-49db-9d0c-597d3d1c5ea2",
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
              "id": "281f7856-8fe9-4a6c-9fca-7c1ec9176303"
            }
          ]
        },
        {
          "id": "78082c73-6c76-480c-81d2-e28147d4af9a",
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
              "id": "e20d9a1f-82c0-4204-a043-85eea5e8c4de"
            }
          ]
        },
        {
          "id": "7f1f756f-d9cc-47cb-8064-5553d20aac7b",
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
              "id": "2e7f6f65-e94b-4b2e-b6e7-2de5f5e6b601"
            }
          ]
        },
        {
          "id": "3350a785-fc6a-4720-91f4-3ef208abb4ef",
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
              "id": "da159c4a-c0c6-4647-831b-7b43e04b9054"
            }
          ]
        },
        {
          "id": "5981d82c-64d9-4cbd-9726-2bc90c52cf16",
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
              "id": "6a90ebb8-25e6-4f59-b07a-d7ae6d29be05"
            }
          ]
        },
        {
          "id": "8c158842-d8e8-429a-98a0-15c2ff9dba45",
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
              "id": "f3fb55f0-f192-4b57-b418-2c89995275c3"
            }
          ]
        },
        {
          "id": "5debfbb5-e0ad-40d9-9d27-acbcf2d29b51",
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
              "id": "0adbc554-b386-498c-8e6b-ded13255f8ec"
            }
          ]
        },
        {
          "id": "505aaf3c-e5ad-4957-8337-a3944fb53a43",
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
              "id": "d1d91672-680c-490c-90fd-d884176b34da"
            }
          ]
        },
        {
          "id": "09a8e7f2-22f8-4582-b53b-b51917e204c0",
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
              "id": "2ec3a993-90bd-4740-b9c1-c497198aa010"
            }
          ]
        }
      ]
    },
    {
      "name": "Listings",
      "item": [
        {
          "id": "8b7483e8-a07f-4572-9b3b-a8fadf809528",
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
              "id": "e0396c91-b775-41bb-bc0b-c8355f25db86"
            }
          ]
        },
        {
          "id": "b9139449-b7b4-48b7-9c27-d2e08c8e1c61",
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
              "id": "c073c86e-b9e9-4e84-826f-beb3959e8b90"
            }
          ]
        },
        {
          "id": "2d53ba57-1817-43eb-bbcc-32a7a1625022",
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
              "id": "3af6efbb-5423-41bd-bf98-498238a0b4d1"
            }
          ]
        },
        {
          "id": "215b19c3-2830-46a2-ac52-6f9a7cdc0fe5",
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
              "id": "d2ff524a-370d-4327-8f0f-5ac5d45bd583"
            }
          ]
        },
        {
          "id": "efd83118-9162-4166-a742-48d4c2528d5e",
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
              "id": "e8876251-137d-4e02-894c-af1ec776d2c6"
            }
          ]
        },
        {
          "id": "4e23bc12-ab77-4955-9949-39bc25be441c",
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
              "id": "8a2bbd4d-670e-4864-a249-20582757e257"
            }
          ]
        },
        {
          "id": "a47e8126-2304-40ea-a4f1-4dd9a20e8bb1",
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
              "id": "0e7e5266-a563-437a-95eb-69e28064f0da"
            }
          ]
        },
        {
          "id": "c7d95157-dfdc-4285-81ec-fcad3a5e2620",
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
              "id": "81debdab-d70c-4cdd-9c6b-8fa4ee7800f8"
            }
          ]
        },
        {
          "id": "c07a3414-7862-4cd5-9017-a1fd52ce6c05",
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
              "id": "fb9f1f7e-d834-47ad-9512-cc6a7db91aec"
            }
          ]
        },
        {
          "id": "764c905d-4d15-40df-8ac7-f058ac4be1ca",
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
              "id": "f56615f0-8d2f-4b46-aece-05054fb67afd"
            }
          ]
        },
        {
          "id": "be0e85d0-1856-4cf0-9556-61e9fc7fedbe",
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
              "id": "651aad68-2637-4669-8a87-6b032a330d5b"
            }
          ]
        },
        {
          "id": "7be234dc-706e-4de2-9edf-e1c5ac1f560f",
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
              "id": "f0fc5775-b4cf-4026-b987-f68fc27c52b0"
            }
          ]
        },
        {
          "id": "83341586-631a-4bd7-9ef5-b9ee66ca3470",
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
              "id": "f109077d-55f0-4e11-a59a-fd30644a6306"
            }
          ]
        }
      ]
    },
    {
      "name": "Shops",
      "item": [
        {
          "id": "52b96ce5-ab03-42c1-a144-fa4cfcfb6426",
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
              "id": "510b5463-8d6f-4b70-a050-785ec6522e4b"
            }
          ]
        },
        {
          "id": "c40fc3cf-999c-46be-a6b5-99894a6b09e3",
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
              "id": "ac0950c5-d1a9-40a2-a870-565c6e421166"
            }
          ]
        },
        {
          "id": "459a55b9-d59d-4823-bcd5-70aec74f58e8",
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
              "id": "7176eaa5-ae67-4345-abae-594941e33554"
            }
          ]
        },
        {
          "id": "0ad9e9c7-e9ff-47b4-a20b-b21b5d614343",
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
              "id": "21bcc612-a62e-4699-891a-6300fced50ed"
            }
          ]
        },
        {
          "id": "d10265be-243c-46ab-a44a-110d9cda721f",
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
              "id": "2af0a3cc-245c-41b9-a56d-abc0490aa034"
            }
          ]
        },
        {
          "id": "01510d6a-7443-4246-8dcc-b60771a9a4ea",
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
              "id": "a724195c-24f2-44ad-aca6-5640261d9874"
            }
          ]
        },
        {
          "id": "8086614a-b998-493b-a6d6-9d2d1e08e62a",
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
              "id": "7266e30e-7476-4187-841d-88da19bcbce1"
            }
          ]
        },
        {
          "id": "c497273c-c13d-4543-8686-95c4896ed289",
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
              "id": "017029ad-365c-4323-815d-6429d1ca7489"
            }
          ]
        },
        {
          "id": "0a14d2b2-e5d9-4e0e-ba09-e9abcb14072b",
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
              "id": "ee7d45bf-2e1b-474b-baf0-24e140dd41ee"
            }
          ]
        },
        {
          "id": "2a9ef5c3-a472-4159-86b5-6da56d596e1a",
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
              "id": "73a387d2-35d7-444a-8749-47d138733539"
            }
          ]
        },
        {
          "id": "e22c7ce1-7d0b-4e32-8e8d-9ef3c0be2496",
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
              "id": "a1a42286-50f9-4189-9078-ab8d3b63a0dd"
            }
          ]
        },
        {
          "id": "680fded1-49ea-4d50-871e-cc143c53a1d6",
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
              "id": "691cdca9-f640-487e-bec9-7d494a6744a0"
            }
          ]
        },
        {
          "id": "7fb260a5-2113-4614-9383-b25ad6290892",
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
              "id": "66bbfa2b-55bf-4567-84ca-a82629689d47"
            }
          ]
        },
        {
          "id": "44063a68-f74c-4147-a507-9941d567a437",
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
              "id": "f2ddc47e-b170-46a6-9740-4302c38d2622"
            }
          ]
        }
      ]
    },
    {
      "name": "Orders",
      "item": [
        {
          "id": "da1a70ea-8699-4a61-808d-adbf50453f96",
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
              "id": "ba79e17d-a145-467c-94ff-db1cd58381e8"
            }
          ]
        },
        {
          "id": "cc3d17f6-1a1e-4b2f-8497-3536ff78a818",
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
              "id": "7787b49c-346d-4100-9216-028bafac8e64"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipts",
      "item": [
        {
          "id": "d45c930b-1782-4801-a31d-734f35817beb",
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
              "id": "d486bc18-a154-4b6c-a064-a3df37a3f843"
            }
          ]
        },
        {
          "id": "81eb9218-ff44-4e53-87e6-6cf646c2c8ea",
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
              "id": "fa961cdd-17df-440f-a191-45f2315a8b8c"
            }
          ]
        },
        {
          "id": "ed61082e-a87b-4c41-9870-28afc533f387",
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
              "id": "7338f670-64a6-4ac3-8a9e-7b410d5ddf3f"
            }
          ]
        }
      ]
    },
    {
      "name": "Regions",
      "item": [
        {
          "id": "17d38890-ad2e-4fee-b8ad-e2e656458be7",
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
              "id": "25e6d050-a631-48c6-84ca-617c773e7054"
            }
          ]
        },
        {
          "id": "df01c809-26e6-43c0-b809-2afa8af39284",
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
              "id": "9f9329e6-f794-4b38-bcb8-e396551623b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Shipping",
      "item": [
        {
          "id": "a0d0c965-005a-43bb-a72a-027aa7f27912",
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
              "id": "01eca546-e91b-4718-bc93-39edecfc0f2c"
            }
          ]
        },
        {
          "id": "55ccdce0-fcd3-4aa9-9b32-590ed2e8b003",
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
              "id": "a216c243-511a-479a-9650-306d3782ad0a"
            }
          ]
        },
        {
          "id": "4a4ae76f-b82c-4a18-bbbd-ffac7b67c10e",
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
              "id": "5be266df-d4a8-40c8-b074-e30c663076f0"
            }
          ]
        },
        {
          "id": "6c033f3c-6c8e-40bb-a528-4dd6c3f2777f",
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
              "id": "be70eb21-64e0-4055-8998-d0530769fa25"
            }
          ]
        },
        {
          "id": "06eb1b58-2a30-4165-a80d-3f060ef17d96",
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
              "id": "b069d5cc-fd5a-4af4-b6bc-f5fe4bc47ace"
            }
          ]
        },
        {
          "id": "821cce38-d2e7-4efd-bd87-fa604e93b717",
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
              "id": "6ae7f0d8-8eb9-4fa4-bf74-dad5804a36ce"
            }
          ]
        },
        {
          "id": "c9791426-4997-4948-b9af-dc2c6a77cfe6",
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
              "id": "b1027acc-e738-4436-b213-cec0f1b6796d"
            }
          ]
        },
        {
          "id": "c270646c-ffef-4fc2-9165-be52d8837306",
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
              "id": "791518f3-62cc-4dd1-8216-bf9f31c0288c"
            }
          ]
        },
        {
          "id": "2772c73d-d170-4f6f-9800-a14289720848",
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
              "id": "df2aa179-a96b-438a-b923-67aa4e1d5b52"
            }
          ]
        },
        {
          "id": "96e0d80c-e73a-4ce8-9659-041776c35a97",
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
              "id": "cb7a2fdc-1554-4c2b-8731-9e9552e00234"
            }
          ]
        },
        {
          "id": "5dc10e8a-3d3b-4054-897a-f820fca12784",
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
              "id": "fd7b3e17-dcdf-4938-80f6-dbc4ca192e7c"
            }
          ]
        },
        {
          "id": "64f109b1-9437-4dd7-a9b9-8773e7fbb1cc",
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
              "id": "d96adeac-dac5-45e8-8eb7-026735c1fae1"
            }
          ]
        }
      ]
    },
    {
      "name": "Sections",
      "item": [
        {
          "id": "81913fef-39f3-451e-b664-3d2126b3b9c9",
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
              "id": "f6287820-cac4-4409-bccd-65b039a4770b"
            }
          ]
        },
        {
          "id": "d8fba292-ef83-492a-b525-a4b273536723",
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
              "id": "08643526-0be6-4f82-882c-597799d124a7"
            }
          ]
        },
        {
          "id": "e03183a0-ed04-4294-a46b-f7b2490dd0eb",
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
              "id": "2b2ea457-53f7-4a5e-b414-36addb8b33cf"
            }
          ]
        },
        {
          "id": "179351e0-93ad-4422-9a01-1f5f1ae31ab7",
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
              "id": "7bb7ec95-bc2d-4a64-987b-d3d36b059acd"
            }
          ]
        }
      ]
    },
    {
      "name": "Categories",
      "item": [
        {
          "id": "c2017904-98d3-457b-a94a-1b8a52951f72",
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
              "id": "289a21a0-43bd-471b-8641-799ccdce0f9d"
            }
          ]
        },
        {
          "id": "90cd245a-0fa6-4c77-94cd-3cfd461f9cad",
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
              "id": "10d3312d-9ea0-4740-aff0-372b06196e1a"
            }
          ]
        },
        {
          "id": "3038cf57-fcaf-4845-a7db-f740059905f8",
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
              "id": "ab9496aa-656b-447c-abf0-2433ca03dbf2"
            }
          ]
        }
      ]
    },
    {
      "name": "Taxonomy",
      "item": [
        {
          "id": "e15beb5b-5d3a-4c0b-a541-396f314cda36",
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
              "id": "65922e84-854a-4798-a8f5-74eeb0a67370"
            }
          ]
        },
        {
          "id": "af8a7984-cad7-4219-93ab-7223db8349c2",
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
              "id": "b709b71a-49e7-469b-a0b7-8d21e858b127"
            }
          ]
        },
        {
          "id": "39905797-76cf-4210-909d-8b499bed2856",
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
              "id": "a3fe46ed-a7d7-4b82-9efc-e0996dc69a00"
            }
          ]
        },
        {
          "id": "eb3ae992-8a59-4a37-9775-6a6141e38402",
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
              "id": "070617ca-22f6-49ae-9817-cafc58485436"
            }
          ]
        },
        {
          "id": "c1905f85-1156-4505-8760-4f58cc78adc5",
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
              "id": "4b825211-51da-4ab7-abc0-488a3219fa36"
            }
          ]
        }
      ]
    },
    {
      "name": "Transactions",
      "item": [
        {
          "id": "396b6a77-a938-4ef1-8a45-353c9580668a",
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
              "id": "922a6f27-a33f-40fe-88c7-b567f9f0a2dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Treasuries",
      "item": [
        {
          "id": "f1e84bfe-68a4-4f7b-812d-208d524b53d4",
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
              "id": "f19131d7-e607-4817-b7dc-cec99236b720"
            }
          ]
        },
        {
          "id": "f16e0fe2-4d23-498a-8beb-87a20e59ce60",
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
              "id": "b7f479d5-0822-4bf8-b5d5-1b1493bc0dbf"
            }
          ]
        }
      ]
    },
    {
      "name": "Payments",
      "item": [
        {
          "id": "d5f3b595-9891-4d53-996f-04208de67ee9",
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
              "id": "5fadcb26-5a80-4b62-ab67-c10137fff293"
            }
          ]
        },
        {
          "id": "8de24a09-8326-4483-adea-9776a1ffc873",
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
              "id": "143fa834-be8a-49bf-9333-238195134343"
            }
          ]
        },
        {
          "id": "e5822fcb-1cf2-46c2-9ad2-4ad5e7337847",
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
              "id": "210e440a-2a9c-4b21-8ada-5da2cd2fee0b"
            }
          ]
        },
        {
          "id": "1b45cc7d-7d60-4d07-b1dc-e8acb94294d0",
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
              "id": "f2eb3a9d-3a14-4b81-8dd4-49946755ace0"
            }
          ]
        }
      ]
    },
    {
      "name": "Featured",
      "item": [
        {
          "id": "7e490db8-db1c-4fbb-acbf-8084bb108d7e",
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
              "id": "b6871d35-9d90-4be7-a59f-3e7376299ffc"
            }
          ]
        },
        {
          "id": "a6215caa-6078-4d64-9117-c406713572f0",
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
              "id": "409ef017-c480-4595-9828-10e61f2816fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "6bcddd21-46bf-4976-ae5f-fb8010bd5f73",
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
              "id": "8707ed7d-18b2-4fd1-a9f2-d5654e13fcfe"
            }
          ]
        }
      ]
    },
    {
      "name": "Server",
      "item": [
        {
          "id": "e6ae29ed-bf14-4f3a-b983-ee13c19a4b42",
          "name": "getServerEpoch",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/server/epoch",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get server time, in epoch seconds notation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c964c57-b444-4195-8342-c939967c2b23"
            }
          ]
        },
        {
          "id": "e8eca90d-f401-4db9-a29b-b627d432503e",
          "name": "getServerPing",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/server/ping",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Check that the server is alive."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5034f18-52ee-4205-bf38-aed0afcc53bf"
            }
          ]
        }
      ]
    }
  ]
}