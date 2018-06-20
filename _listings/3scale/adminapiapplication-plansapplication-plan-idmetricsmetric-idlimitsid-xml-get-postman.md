{
  "info": {
    "name": "3Scale Account Management API Limit Read",
    "_postman_id": "bd80c71d-584c-4f3e-8211-7d06efecdabd",
    "description": "Limit read.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "c2b9f320-e5ce-4281-b7eb-56dfccf1156e",
          "name": "account",
          "request": {
            "url": "http://su1.3scale.net/admin/api/accounts.xml?page=%7B%7D&per_page=%7B%7D&provider_key=%7B%7D&state=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5b9737a-ae48-41eb-873a-4079d92af754"
            }
          ]
        },
        {
          "id": "e0481cc2-36e9-44ea-a1eb-826a6eb3bdeb",
          "name": "account",
          "request": {
            "url": "http://su1.3scale.net/admin/api/accounts/find.xml?email=%7B%7D&provider_key=%7B%7D&username=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account find."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71b2a860-9d2f-4a7f-b995-e55300caddc5"
            }
          ]
        },
        {
          "id": "a641f16a-3c07-47c9-b9d4-e55e9af8f518",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/messages.xml"
              ],
              "query": [
                {
                  "key": "body",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Account message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6288ea0-f2f8-48cb-8eac-48a066789fd4"
            }
          ]
        },
        {
          "id": "7fcc90a0-0c5e-4572-b13b-e097b33198ae",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/plan.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account fetch account plan."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67ed2d5f-911a-41ec-85dd-d13579341bce"
            }
          ]
        },
        {
          "id": "23a3dbbc-b635-49d9-b295-b7a22a286b51",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58c8bc9a-be4b-4eea-8f5a-297a3160b6dc"
            }
          ]
        },
        {
          "id": "151eba88-1710-4bde-a0b6-ee230133256e",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id.xml"
              ],
              "query": [
                {
                  "key": "additional_fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "org_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Account update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7685721d-8164-423b-b025-57257bf0c7fe"
            }
          ]
        },
        {
          "id": "f6d54a4e-8c8a-4b80-a1e3-2eaa64a41389",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Account delete ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a02f27d-1e27-4e1f-a0fa-125992da0b31"
            }
          ]
        },
        {
          "id": "84c018c9-3eaf-4e71-83ff-2bd86d649f31",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id/approve.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Account approve."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5489254-640e-42fd-b521-634acc46aa00"
            }
          ]
        },
        {
          "id": "c6da6985-ac23-4d3d-852c-b56ff4fc8397",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id/change_plan.xml"
              ],
              "query": [
                {
                  "key": "plan_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Account change plan."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b3a7810-faac-4aa5-a3c5-f473e17c159a"
            }
          ]
        },
        {
          "id": "492a4a29-e39a-43cc-b974-bdfcc0bd6289",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id/credit_card.xml"
              ],
              "query": [
                {
                  "key": "billing_address_address",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "billing_address_city",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "billing_address_country",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "billing_address_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "billing_address_phone",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "billing_address_state",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "billing_address_zip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "credit_card_authorize_net_payment_profile_token",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "credit_card_expiration_month",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "credit_card_expiration_year",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "credit_card_partial_number",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "credit_card_token",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Account set credit card."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da9f6bbd-7877-4bb1-a545-34e658da0706"
            }
          ]
        },
        {
          "id": "7e8fbe5d-29f1-46f0-9dd7-4d08e06a9cc3",
          "name": "account1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id/credit_card.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Account delete credit card."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d15a626d-b30c-4da3-867c-23b3a4c42499"
            }
          ]
        },
        {
          "id": "10d23f38-db8c-4d93-8124-ba6b4a8e3ee8",
          "name": "account1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id/make_pending.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Account reset to pending."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "896c8295-a692-435e-8bd2-c8dd1557d4a7"
            }
          ]
        },
        {
          "id": "1d01703f-45f0-43b0-9c31-4ed43d4ef0b4",
          "name": "account2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id/reject.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Account reject."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63f4f728-b3ca-4d88-b560-4870a6111d6a"
            }
          ]
        },
        {
          "id": "9bce8b09-7f99-48ef-8e71-02ea0490cd7a",
          "name": "account_plan",
          "request": {
            "url": "http://su1.3scale.net/admin/api/account_plans.xml?provider_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account plan list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9419546-292c-43fe-bc3b-8da424774bdb"
            }
          ]
        },
        {
          "id": "d7b0875e-a2ac-4328-94c3-bd01c187cb93",
          "name": "account_plan",
          "request": {
            "url": "http://su1.3scale.net/admin/api/account_plans.xml?name=%7B%7D&provider_key=%7B%7D&system_name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Account plan create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "868ed77f-123c-4600-ba08-ff695358730c"
            }
          ]
        },
        {
          "id": "64810cd1-8c1c-4f84-955c-f9614471eb88",
          "name": "account_plan_feature",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/account_plans/:account_plan_id/features.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_plan_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account plan feature list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aac674fc-5f9f-47a8-913d-fa046aba48f6"
            }
          ]
        },
        {
          "id": "c7d2e463-d19d-45ea-85c8-a0df86f8c6f1",
          "name": "account_plan_feature",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/account_plans/:account_plan_id/features/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_plan_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Account plan features create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0f51f5f-e9fd-413c-8302-6c8be8c88c7f"
            }
          ]
        },
        {
          "id": "bcb29efe-6d8a-48c4-904a-c2bdfd3bc909",
          "name": "account_plan_feature",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/account_plans/:account_plan_id/features/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_plan_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Account plan features delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e132be5a-6f29-42b6-89d6-bd5e1e587e16"
            }
          ]
        },
        {
          "id": "a7bd01b7-7ec9-49e8-a051-245c6d272aeb",
          "name": "account_plan",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/account_plans/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account plan read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5247d93-f22f-41fc-aff4-e501722d47fd"
            }
          ]
        },
        {
          "id": "831da13d-3ed7-433f-9504-9c8326d94121",
          "name": "account_plan",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/account_plans/:id.xml"
              ],
              "query": [
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Account plan update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f98ba623-d14a-46ad-9ca2-e938a22a720c"
            }
          ]
        },
        {
          "id": "a216781c-de77-4f4a-ac51-63d8ed6efede",
          "name": "account_plan",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/account_plans/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Account plan delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcec3f11-83ec-4929-a80a-e148a3162ff5"
            }
          ]
        },
        {
          "id": "d6927576-578e-430f-8386-86fba9657928",
          "name": "account_plan",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/account_plans/:id/default.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Account plan set to default."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49e28831-ea0c-46f6-bf22-8cc8da2185bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "392c86f8-05c3-49f9-ab26-5636a8198cb0",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "693ffd76-124e-4079-a1dc-cefd9121585e"
            }
          ]
        },
        {
          "id": "cc4f7aad-bb68-4f2b-adba-1ce9149ad281",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications.xml"
              ],
              "query": [
                {
                  "key": "additional_fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "plan_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Application create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87e17016-f737-46eb-9cef-5bf2a2814a2a"
            }
          ]
        },
        {
          "id": "f2077b06-9d1d-436b-b16e-c393e9b40297",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:application_id/keys.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application key list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fd689ed-5539-4b0a-91d2-186710d210ce"
            }
          ]
        },
        {
          "id": "34454e8b-a037-4353-8157-b9c132032bbe",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:application_id/keys.xml"
              ],
              "query": [
                {
                  "key": "key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Application key create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "447aecb5-429a-4bb0-b94f-0f4cb7f99a63"
            }
          ]
        },
        {
          "id": "ae9a4e71-6a61-4df3-a691-19b27e82bb58",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:application_id/keys/:key.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Application key delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "361be01d-5ba1-4163-b605-353da612edc8"
            }
          ]
        },
        {
          "id": "0f453fbb-f701-4567-9729-763fb52f7cee",
          "name": "application1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:application_id/referrer_filters.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application referrer filter list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8928de9-6b78-443c-b766-3273af01c461"
            }
          ]
        },
        {
          "id": "18b5b9f6-5e97-411f-9939-e516da1a11d2",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:application_id/referrer_filters.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "referrer_filter",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Application referrer filter create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae55ec28-0105-427c-bdf2-e871c121533a"
            }
          ]
        },
        {
          "id": "4058737d-42d7-4ff1-b265-c658c0aa3f3b",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:application_id/referrer_filters/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Application referrer filter delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e553423-eb2a-4ea5-b4fd-f7f53f15b91f"
            }
          ]
        },
        {
          "id": "f480baee-93a5-456d-971e-d8ad2e1e7c89",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32af7291-71dc-439f-a3e4-0be2b5f10bd8"
            }
          ]
        },
        {
          "id": "b0a2fe05-b354-43b9-b6ad-cbb69e4177ac",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id.xml"
              ],
              "query": [
                {
                  "key": "additional_fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e24993a4-2ccf-4530-8345-527f449317b6"
            }
          ]
        },
        {
          "id": "ec785366-5f89-419a-80e9-58db091608a3",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id/accept.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application accept."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f92a273c-14cb-444e-be9a-c350b1daf3c6"
            }
          ]
        },
        {
          "id": "340f10f7-4924-4bc8-8f2d-e4c38a37189d",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id/change_plan.xml"
              ],
              "query": [
                {
                  "key": "plan_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application change plan."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4718b98-a67f-49b8-81f7-e7ade232473c"
            }
          ]
        },
        {
          "id": "6a5131cc-1cd6-4e84-832a-968cd9efc0fd",
          "name": "application1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id/customize_plan.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application create plan customization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6318776d-04f1-4e00-85b1-dd851d0531ba"
            }
          ]
        },
        {
          "id": "e7d1d6af-7cee-4c01-9288-dcb72831c51d",
          "name": "application2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id/decustomize_plan.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application delete plan customization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ad9cd2c-e19e-48a1-b15d-601c7477fc6f"
            }
          ]
        },
        {
          "id": "aa7fbe97-0881-4f56-9949-92d28302a182",
          "name": "application3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id/resume.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application resume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b97a03a4-4a58-4038-9dc7-7ad9e5518b7b"
            }
          ]
        },
        {
          "id": "ae94ea02-079c-4266-a3ad-f93003e9c4f7",
          "name": "application4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id/suspend.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application suspend."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9207a4be-70cc-4300-b84b-0929bdd42262"
            }
          ]
        },
        {
          "id": "337dbbe5-683b-4f90-b54c-372832eac02f",
          "name": "application",
          "request": {
            "url": "http://su1.3scale.net/admin/api/applications.xml?active_since=%7B%7D&inactive_since=%7B%7D&page=%7B%7D&per_page=%7B%7D&provider_key=%7B%7D&service_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application list (all services)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18b15079-3716-4acd-8a48-7bfba0f0cd7b"
            }
          ]
        },
        {
          "id": "eb337ba7-e3a4-46cc-8375-8b9a6e71e71c",
          "name": "application",
          "request": {
            "url": "http://su1.3scale.net/admin/api/applications/find.xml?application_id=%7B%7D&app_id=%7B%7D&provider_key=%7B%7D&user_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application find."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cb67a91-2ce6-4c47-8ab1-1f1824f3be70"
            }
          ]
        },
        {
          "id": "160cae80-4d03-4f8a-b93a-d3fcc8bddedf",
          "name": "application_plan",
          "request": {
            "url": "http://su1.3scale.net/admin/api/application_plans.xml?provider_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application plan list (all services)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51827674-cc39-42a6-b2f9-ee6a33c2d484"
            }
          ]
        },
        {
          "id": "038da79c-122a-426a-a01f-e549f37d7877",
          "name": "application_plan_feature",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/application_plans/:application_plan_id/features.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application_plan_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application plan feature list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a056a5f-1f87-4bb1-a780-b5c14fea5dd8"
            }
          ]
        },
        {
          "id": "461cd0ce-7030-4e80-81d6-c69fb3c00d2a",
          "name": "application_plan_feature",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/application_plans/:application_plan_id/features.xml"
              ],
              "query": [
                {
                  "key": "feature_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application_plan_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Application plan feature create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17e7bc9d-721e-411c-9f8b-e2d4875fadfc"
            }
          ]
        },
        {
          "id": "1d54c94b-9d69-4634-98d0-189c3920c2ce",
          "name": "application_plan_feature",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/application_plans/:application_plan_id/features/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application_plan_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Application plan feature delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bde3c5c-7aaa-4501-a767-b2f5b8e6124c"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "92bd6469-acec-4c43-8072-160865c3fc8c",
          "name": "user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "role",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce2baa6f-6701-4b6f-88fe-23fb6d687fcb"
            }
          ]
        },
        {
          "id": "da564a7f-2ad1-4cbd-a622-2f2e6f06c142",
          "name": "user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users.xml"
              ],
              "query": [
                {
                  "key": "additional_fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "password",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "username",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "User create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "135ba9ea-7375-42fc-bb04-c5b3236eb8ce"
            }
          ]
        },
        {
          "id": "16633e33-bd97-4b0d-996e-419bcc271b71",
          "name": "user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "225c7a33-85ad-46aa-a5a4-1a723526a25c"
            }
          ]
        },
        {
          "id": "7ec7acd9-d8c9-4b50-914f-9587ba1bac32",
          "name": "user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id.xml"
              ],
              "query": [
                {
                  "key": "additional_fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "password",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "username",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "User update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c248cb1-5246-4df2-9c63-d8662a1f7054"
            }
          ]
        },
        {
          "id": "d8dcc027-d822-4305-a0fd-844580376bae",
          "name": "user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "User delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ceef7f0c-ec09-4e91-9027-86a90bd72fa5"
            }
          ]
        },
        {
          "id": "2a8e8f03-e0d2-43b1-b577-e14e8b81da96",
          "name": "user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id/activate.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "User activate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ddbcc202-343d-4c9a-95bc-c73b94387e16"
            }
          ]
        },
        {
          "id": "5d2dd714-e24e-45a1-af84-105cd9a0955d",
          "name": "user1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id/admin.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "User change role to admin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da30405f-4933-4a9d-a38d-da67069af20b"
            }
          ]
        },
        {
          "id": "ca86b6ff-5b74-4b04-a6bc-614e585d46a2",
          "name": "user2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id/member.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
    