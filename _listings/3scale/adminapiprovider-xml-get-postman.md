{
  "info": {
    "name": "3Scale Account Management API Account Read",
    "_postman_id": "45939fde-bd12-48e8-a86e-d8d8d86eff62",
    "description": "Account read.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "8a1aa0f7-6484-41e4-beb0-7277188d54fd",
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
              "id": "4cc66c6f-2ae7-4670-919e-eab23e0add38"
            }
          ]
        },
        {
          "id": "1449b1e9-50c4-48d0-8865-bc10115fca56",
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
              "id": "13b888e4-688b-4bd1-870c-789a39df37bd"
            }
          ]
        },
        {
          "id": "ddbf8944-8e0d-4be7-9c10-2d4d89f34ce4",
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
              "id": "b3275aec-8af8-4396-a8c1-7e7cafdd3bd2"
            }
          ]
        },
        {
          "id": "a4a5a985-51b6-4cb5-a099-ba5e415307c1",
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
              "id": "1bdc1a43-2758-4b9d-807b-daf0f952c2c4"
            }
          ]
        },
        {
          "id": "7ff5be46-c345-4725-bc45-1a94e44f73f6",
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
              "id": "5eb2882c-d0bf-4f66-97f1-d12e57af1122"
            }
          ]
        },
        {
          "id": "fe3af840-54e7-41e8-bdf1-3392d5c53957",
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
              "id": "459dfab5-1bcf-4209-99b1-64557899572f"
            }
          ]
        },
        {
          "id": "2c3efe71-39f7-44a7-bb5b-0407137a0776",
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
              "id": "d4709955-036c-407d-9237-965bd33b8961"
            }
          ]
        },
        {
          "id": "1cef6ab6-c64e-4d3f-a190-8f63608deb3b",
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
              "id": "63dd2621-4798-4544-b229-b14db8668806"
            }
          ]
        },
        {
          "id": "a39253c7-a6f4-43ad-a8e5-1ee8de9a6b03",
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
              "id": "1d799782-1333-456a-9131-473bdd640be7"
            }
          ]
        },
        {
          "id": "d389ce27-d199-4264-ad42-0fffbfa9e30a",
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
              "id": "e68d78bf-06e1-4816-aa8c-de52f24dc4db"
            }
          ]
        },
        {
          "id": "d57daca5-a89d-4fac-a761-19b0ffee70d7",
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
              "id": "725c1137-b745-4229-8e84-db2ae5da1a8b"
            }
          ]
        },
        {
          "id": "2ee1cade-94e6-42e8-9dd3-47d97339df63",
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
              "id": "8a61e797-a8fc-4f80-a462-e96b1cf134a5"
            }
          ]
        },
        {
          "id": "3cf03701-98b3-4c9d-aeeb-22936c61cc6c",
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
              "id": "3aa7ec9e-c273-4bdf-acea-19226c938b30"
            }
          ]
        },
        {
          "id": "5a30b1b6-3ce4-465e-8298-768e7483c3c2",
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
              "id": "975aef81-44e8-4df6-a49e-f3282918441b"
            }
          ]
        },
        {
          "id": "c9dc3804-db73-461a-b9ef-6c75f6661f0e",
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
              "id": "84aff433-36d6-4769-8de5-1058563665dd"
            }
          ]
        },
        {
          "id": "beb6493e-1cd4-422a-894d-0d2fb85da702",
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
              "id": "07889b39-36a3-45a8-8add-d8342b1eef7f"
            }
          ]
        },
        {
          "id": "4f98128d-e944-427f-80d0-e86fc031f2b9",
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
              "id": "4fe34bb8-9e56-41c3-bc51-af977024a199"
            }
          ]
        },
        {
          "id": "541cd351-08cd-400f-aa13-47e0a54d5ef6",
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
              "id": "4d143430-fd11-48fe-9208-1adf8dc135b5"
            }
          ]
        },
        {
          "id": "b7af3c43-305a-4508-9c80-2745950182bc",
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
              "id": "42228fc9-b5bf-4293-9c79-bb4657cf6a62"
            }
          ]
        },
        {
          "id": "f53cfc69-b4bf-4526-9d34-f41457488e96",
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
              "id": "2f3c5002-a809-48a4-b5c7-714fe8d1ba18"
            }
          ]
        },
        {
          "id": "53a4a62b-cae5-46e5-8a26-c6ddf330e800",
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
              "id": "dcad771a-c988-4b60-8b14-c4c328d9d494"
            }
          ]
        },
        {
          "id": "86085ab2-9458-40f6-a46b-823395528fb1",
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
              "id": "88180a42-7bbd-45ce-bd58-300b90f5268f"
            }
          ]
        },
        {
          "id": "da047a02-2c65-40cf-b23c-56056037551a",
          "name": "account_feature",
          "request": {
            "url": "http://su1.3scale.net/admin/api/features.xml?provider_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account feature list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab716cfb-9cce-4dc5-a1c5-ab12159f5561"
            }
          ]
        },
        {
          "id": "e52879e9-8846-429f-8abe-4b7915f5a4b6",
          "name": "account_feature",
          "request": {
            "url": "http://su1.3scale.net/admin/api/features.xml?name=%7B%7D&provider_key=%7B%7D&system_name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Account feature create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b4ce1ec-9d1e-4db0-adfe-4d4b47bd74e9"
            }
          ]
        },
        {
          "id": "8ce59fe5-b7a9-4e8b-abb7-d36d6d0e94ce",
          "name": "account_feature",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/features/:id.xml"
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
            "description": "Account feature read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1e08c4f-55e0-4874-a5e6-11476f70f6c9"
            }
          ]
        },
        {
          "id": "0a6cb8cb-820b-490e-9a63-266a297f0234",
          "name": "account_feature",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/features/:id.xml"
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
            "description": "Account feature update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d265563a-6554-46b0-9cc3-cf9f7957f12f"
            }
          ]
        },
        {
          "id": "cd729d38-32ca-4260-bbdf-3f7a0e74b289",
          "name": "account_feature",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/features/:id.xml"
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
            "description": "Account feature delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "164fc75b-a9c6-41dd-a940-928b645d0bd2"
            }
          ]
        },
        {
          "id": "0518ae8f-146c-4526-85c3-f8096bcf1468",
          "name": "account",
          "request": {
            "url": "http://su1.3scale.net/admin/api/provider.xml",
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
              "id": "a2630506-6beb-4484-9b42-abc9200a7ccd"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "678a6f5b-d179-405d-9e7d-943b1ddfc52b",
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
              "id": "61e9b39f-4619-43e0-81ce-6914312cabf2"
            }
          ]
        },
        {
          "id": "8442664a-1e63-4995-a932-013d640c3adb",
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
              "id": "fe0bb625-2562-4c09-b947-047e0eb7e278"
            }
          ]
        },
        {
          "id": "55d363f9-e98d-4381-a68d-66c539b69e68",
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
              "id": "28ce17f5-1dfe-4930-a561-519de454f265"
            }
          ]
        },
        {
          "id": "2eb90125-cfa5-43d4-b3dc-45a220a60617",
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
              "id": "bd36f78f-9153-4af8-b33b-5e1977313453"
            }
          ]
        },
        {
          "id": "fde8f7cc-301a-4a15-b645-be3513534588",
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
              "id": "05f89fd9-a24c-497a-b3c0-2ed886591389"
            }
          ]
        },
        {
          "id": "53a114de-5968-4184-8018-06ebcd7bff68",
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
              "id": "d25ac52a-3626-47a2-b627-af74d2a95b52"
            }
          ]
        },
        {
          "id": "d1cba1dc-a1d5-4fee-8188-6b066c6573c3",
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
              "id": "75a15b36-de1d-4300-b23d-a6aa4ce685dc"
            }
          ]
        },
        {
          "id": "53a1d46a-cc56-4b8d-9099-1f747d1be1aa",
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
              "id": "b0972c18-3518-43a7-bd67-cf119929ed90"
            }
          ]
        },
        {
          "id": "9126b290-d633-45ec-9c5c-1c3e4419430e",
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
              "id": "8c7c0a31-2b48-4bf4-93db-e5590367ef64"
            }
          ]
        },
        {
          "id": "d287b06e-e521-4a81-85a4-fd969511629b",
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
              "id": "6e6baa60-4a89-4eea-b8e0-5de0a94da5fb"
            }
          ]
        },
        {
          "id": "fef21879-7b8a-4618-8454-4d36d8506b56",
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
              "id": "23ae3c7e-3fe0-43b1-adbd-e6a9d1364d1e"
            }
          ]
        },
        {
          "id": "49b71d36-b363-424e-ac83-14dd357028d5",
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
              "id": "2f8ccf2b-8ffa-4e04-8c57-cc5887466709"
            }
          ]
        },
        {
          "id": "42161264-42a2-4c4e-8568-02a13cce1edb",
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
              "id": "e14af0fc-ba42-40ba-9503-e775407d0ed2"
            }
          ]
        },
        {
          "id": "139ad76d-076d-4315-b174-20d32ccca077",
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
              "id": "cea3adc9-c891-4648-aad3-2270462672d2"
            }
          ]
        },
        {
          "id": "000cd93d-7857-4310-8cab-bfca831f7b3e",
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
              "id": "d3c613a0-bed1-4251-ab26-151e209c8086"
            }
          ]
        },
        {
          "id": "dd562f1f-faca-46fc-b279-62edd02443ca",
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
              "id": "000b2d9f-5749-4820-9120-78fcdb2be054"
            }
          ]
        },
        {
          "id": "fb7cb290-95cb-4ee8-ab02-2cc866de0aab",
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
              "id": "aeb620fd-7073-43bc-b015-c0d36789c7f4"
            }
          ]
        },
        {
          "id": "4d7b6f32-af1e-4a6f-9c59-265fc6ff6e21",
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
              "id": "d7c7c3bf-cea7-4b4b-be9b-0d555da5dbdf"
            }
          ]
        },
        {
          "id": "af7321e8-feb4-4f7e-af0f-b28ec68dd9fe",
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
              "id": "2dc4d159-59e2-41fb-b1e8-026a48f89ae1"
            }
          ]
        },
        {
          "id": "8ee3ccf4-5796-4aaf-824a-77b75d595b65",
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
              "id": "d5724a92-25f6-4f85-b5b4-278ffbafb7d7"
            }
          ]
        },
        {
          "id": "a1d7c20e-20d0-4554-a2d6-2ec2c815c009",
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
              "id": "d71e406e-1816-4332-8e85-19bd687523ca"
            }
          ]
        },
        {
          "id": "3c537a83-603d-4105-a9ca-884d8cedf4af",
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
              "id": "beae7e55-3e8d-4e4c-8031-f52ee93f9b36"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "104ac8ca-4cdd-4a64-859a-037ac0c31035",
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
              "id": "cdb5b87e-e7e1-4482-97c0-18d88f71ca83"
            }
          ]
        },
        {
          "id": "6657ec2e-00ed-40e8-b8ca-dec1cdb29a95",
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
              "id": "b9ca6a57-5c1a-482e-9ff5-d501b44dd9f5"
            }
          ]
        },
        {
          "id": "5e53ebcb-dff8-4fb2-85bf-dd249ff4da40",
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
              "id": "ef353adf-6c2c-4725-8235-f41705237884"
            }
          ]
        },
        {
          "id": "56026325-5e3a-4858-9646-fe11981242ae",
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
              "id": "2cf5a902-a62b-498c-9c09-8b7d4001152e"
            }
          ]
        },
        {
          "id": "91eaf1f1-b175-4fce-86c3-e236a3a83641",
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
              "id": "2353ae5d-1c9a-4373-8c9e-a9411a1af9d5"
            }
          ]
        },
        {
          "id": "9e47946e-789f-4733-bbae-ee943f35cad1",
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
              "id": "51b4bbf8-d170-4087-bfdb-be5324c55dc9"
            }
          ]
        },
        {
          "id": "04e2bc1a-70da-4c9e-96e2-44e38736bc79",
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
              "id": "acf23cf7-d300-45fe-bf4f-0cd578b2b0a4"
            }
          ]
        },
        {
          "id": "eec6944f-a037-48ed-b317-4ff3229f2ada",
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
            "description": "User change role to member."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59f872f3-c98c-4afb-abe0-e973d587f242"
            }
          ]
        },
        {
          "id": "f1b238a0-e1e3-401c-8a69-bcdd2a422d7d",
          "name": "user3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id/suspend.xml"
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
            "description": "User suspend."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8458005d-25db-4deb-9517-aa772318f4ba"
            }
          ]
        },
        {
          "id": "63549c0b-213e-4beb-b361-613a397c4d98",
          "name": "user4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id/unsuspend.xml"
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
            "description": "User unsuspend."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e409c736-7be4-4466-aff9-1d6e995fbc5b"
            }
          ]
        }
      ]
    },
    {
      "name": "ActiveDocs",
      "item": [
        {
          "id": "84383a0e-1dc6-493f-a396-a0bda5b486f3",
          "name": "active_docs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/active_docs/:id.xml"
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
            "description": "Activedocs json spec update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3129ee0a-8772-47f1-b1a3-41077809935c"
            }
          ]
        }
      ]
    },
    {
      "name": "Limits",
      "item": [
        {
          "id": "73ea887c-4008-4482-9ded-d2c7f38598d5",
          "name": "application_plan_limits",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/application_plans/:application_plan_id/limits.xml"
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
            "description": "Limits list per application plan."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc144c58-3e43-4af5-a6d3-980d8c767ffb"
            }
          ]
        }
      ]
    },
    {
      "name": "Limit",
      "item": [
        {
          "id": "2c565d81-6dfb-4194-b34a-ebd9eae615f0",
          "name": "application_plan_limit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/application_plans/:application_plan_id/metrics/:metric_id/limits.xml"
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
                  "id": "metric_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Limit list per metric."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f92ff47-3854-48d8-b1be-12a5615a54fc"
            }
          ]
        },
        {
          "id": "eb4b8dd5-b710-48fe-a465-9acc1b104f01",
          "name": "application_plan_limit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/application_plans/:application_plan_id/metrics/:metric_id/limits.xml"
              ],
              "query": [
                {
                  "key": "period",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "value",
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
                  "id": "metric_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Limit create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffd032f4-5f9a-4fbc-b41e-c9d022f3736a"
            }
          ]
        },
        {
          "id": "13252db0-17e6-4708-b52a-7573f6f089e6",
          "name": "application_plan_limit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/application_plans/:application_plan_id/metrics/:metric_id/limits/:id.xml"
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
                },
                {
                  "id": "metric_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Limit read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43eab905-8a71-4779-8626-4dde332d3bdc"
            }
          ]
        },
        {
          "id": "07ca2d42-5099-4068-a7d2-b085bb86141a",
          "name": "application_plan_limit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/application_plans/:application_plan_id/metrics/:metric_id/limits/:id.xml"
              ],
              "query": [
                {
                  "key": "period",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "value",
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
                },
                {
                  "id": "metric_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Limit update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bf4731e-19f9-4d71-bc0d-13b940eff940"
            }
          ]
        },
        {
          "id": "dbc08a62-e147-4c62-9dd0-13ac1d0adfe0",
          "name": "application_plan_limit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/application_plans/:application_plan_id/metrics/:metric_id/limits/:id.xml"
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
                },
                {
                  "id": "metric_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Limit delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e973b4f-29fc-48a3-b1a7-934a41301f9b"
            }
          ]
        },
        {
          "id": "63a08a05-3788-402d-8f72-83650ad88ae2",
          "name": "end_user_plan_limit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/end_user_plans/:end_user_plan_id/metrics/:metric_id/limits.xml"
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
                  "id": "end_user_plan_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "metric_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Limit list for end user plans ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe5f57d3-5ccd-4485-8031-34aed07c26b8"
            }
          ]
        },
        {
          "id": "ed3f76b0-86f2-4246-bb19-e12f19a5dd83",
          "name": "end_user_plan_limit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/end_user_plans/:end_user_plan_id/metrics/:metric_id/limits.xml"
              ],
              "query": [
                {
                  "key": "period",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "value",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "end_user_plan_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "metric_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Limit create for end user plans."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62faa8ef-293f-49f6-a994-2d5063fc4a1e"
            }
          ]
        },
        {
          "id": "eb732131-3474-4a37-b97b-0c7b80fb32a7",
          "name": "end_user_plan_limit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/end_user_plans/:end_user_plan_id/metrics/:metric_id/limits/:id.xml"
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
                  "id": "end_user_plan_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "metric_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Limit read for end user plans."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd892ea7-9adb-41a4-9f5d-1aca569a6b8d"
            }
          ]
        },
        {
          "id": "9c050948-295b-4aa7-91c6-0851ca37353d",
          "name": "end_user_plan_limit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/end_user_plans/:end_user_plan_id/metrics/:metric_id/limits/:id.xml"
              ],
              "query": [
                {
                  "key": "period",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "value",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "end_user_plan_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "metric_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Limit update for end user plans."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa089ec2-a0be-4366-993d-d4330eda2cb2"
            }
          ]
        },
        {
          "id": "19d339ff-0574-43ec-a402-dcc22eab5975",
          "name": "end_user_plan_limit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/end_user_plans/:end_user_plan_id/metrics/:metric_id/limits/:id.xml"
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
                  "id": "end_user_plan_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "metric_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Limit delete for end user plans."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ece8d35-5983-4bb2-b5a3-fa9c842d574f"
            }
          ]
        }
      ]
    },
    {
      "name": "Pricing",
      "item": [
        {
          "id": "e39faa77-dfe7-40be-b425-d72d92b1c36b",
          "name": "application_plan_pricing_rules",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/application_plans/:application_plan_id/metrics/:metric_id/pricing_rules.xml"
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
                  "id": "metric_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Pricing rules list per metric."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bef9210-d224-4971-a965-5846a1a68209"
            }
          ]
        },
        {
          "id": "6f04ddac-4034-46dd-8cdb-3c4668a48322",
          "name": "application_plan_pricing_rules",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/application_plans/:application_plan_id/pricing_rules.xml"
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
            "description": "Pricing rules list per application plan."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66147b19-8f1c-40e9-af89-0a6f119b628d"
            }
          ]
        }
      ]
    },
    {
      "name": "End",
      "item": [
        {
          "id": "27a9abed-36aa-49c2-83a5-c61fdc41d43f",
          "name": "end_user_plan",
          "request": {
            "url": "http://su1.3scale.net/admin/api/end_user_plans.xml?provider_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "End user plan list (all services)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b0223cf-2b6f-401f-8f3e-30912d0580b8"
            }
          ]
        }
      ]
    },
    {
      "name": "Nginx",
      "item": [
        {
          "id": "7c4796f8-6aad-4df0-8fac-ec943166da5e",
          "name": "nginx",
          "request": {
            "url": "http://su1.3scale.net/admin/api/nginx.zip?provider_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Nginx configuration files."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16644f40-61b8-415a-b50f-65ad0ee30c87"
            }
          ]
        }
      ]
    }
  ]
}