{
  "info": {
    "name": "3Scale Account Management API Account Feature Create",
    "_postman_id": "76eb6241-f415-418d-8cf1-44521f3f26f4",
    "description": "Account feature create.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "393f5fb4-e357-483c-a277-d6198d6ad43d",
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
              "id": "1468e6a2-89e3-4b23-a40f-ad512344efa9"
            }
          ]
        },
        {
          "id": "c0a6c41d-b02e-40c3-93e7-cf86e3ba4674",
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
              "id": "155c8968-181d-417e-a587-99e98480af20"
            }
          ]
        },
        {
          "id": "95ae6633-e016-45af-873c-d963eefd8b69",
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
              "id": "347e5923-4825-4453-b7eb-592f0f2b2a03"
            }
          ]
        },
        {
          "id": "44541267-31c8-4f06-bebd-3251b12ce806",
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
              "id": "4be18729-492e-4159-ab1c-6aa7ab358a47"
            }
          ]
        },
        {
          "id": "9e23349e-af92-42a2-ad37-e3452e85a947",
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
              "id": "46ddf016-0f36-47ef-b775-c8a5cf164718"
            }
          ]
        },
        {
          "id": "d0d28063-658b-43fe-bb71-39f7f97b267c",
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
              "id": "fed5bf68-f5a4-4517-a6c4-60919f6f0a66"
            }
          ]
        },
        {
          "id": "7ce3c415-ca02-47eb-bad9-1d23ba0fc8ea",
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
              "id": "1080c0c8-1d99-4be6-9b34-9c48cfa3ace4"
            }
          ]
        },
        {
          "id": "cc9d7a01-08dc-4ab3-b9df-6538462e3c65",
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
              "id": "84851bf7-2ff0-483d-a221-c67d517b22a5"
            }
          ]
        },
        {
          "id": "7d19cf78-4b71-404e-b4b6-c2ad81382033",
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
              "id": "e901cbb7-a3b8-46b4-baee-ef689dbeaca0"
            }
          ]
        },
        {
          "id": "739e88f6-1fff-43ff-8b31-96c5c56dfa49",
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
              "id": "eaa8dd90-2a03-4974-8fff-87294e90df11"
            }
          ]
        },
        {
          "id": "991cc3dc-3e7a-460d-be0f-bbd173b89843",
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
              "id": "3e000fb3-083f-43c6-92e1-44826fd36a5a"
            }
          ]
        },
        {
          "id": "90b6824f-db9f-4008-9640-7f53c56032f9",
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
              "id": "2a47802e-6dc1-433b-96e6-411ea9725918"
            }
          ]
        },
        {
          "id": "ff9ae503-430a-48e7-916e-3c3821356358",
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
              "id": "6383e5dd-20f2-4de6-9fa8-e2da0030839a"
            }
          ]
        },
        {
          "id": "7345508f-a226-4dd0-964d-772a7082dd6e",
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
              "id": "d11b827b-6bc1-4297-96f9-9e8ed780cdbe"
            }
          ]
        },
        {
          "id": "8c54c8b4-9322-43a8-89d9-896aebcc4dce",
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
              "id": "0f47f355-7f02-4592-b702-2f59a439ec1f"
            }
          ]
        },
        {
          "id": "280d3571-e37e-4313-a01b-d55c179cd28f",
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
              "id": "303e909d-3bda-4831-9072-3e671a585463"
            }
          ]
        },
        {
          "id": "9e7fd460-ae34-4b7c-807e-76a316af1916",
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
              "id": "4c0da7f6-6562-4624-8666-b13494359430"
            }
          ]
        },
        {
          "id": "39c0626c-073f-4703-a1a7-9aac8f15eeb7",
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
              "id": "fae7544b-14a6-4420-b3b0-a652879055f4"
            }
          ]
        },
        {
          "id": "4dc67435-0e63-4e38-9560-830b296d2c90",
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
              "id": "bca873d7-31be-444e-8bab-5965a4faa6eb"
            }
          ]
        },
        {
          "id": "aeb9942b-f569-4ee5-997c-136f321f3db4",
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
              "id": "ae594af3-d460-44aa-b3ec-6460909689e4"
            }
          ]
        },
        {
          "id": "5310cbd6-4c6d-42ba-86af-fd62e668837c",
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
              "id": "b4e3618a-33b3-4e8d-830c-16c45ed2bcb6"
            }
          ]
        },
        {
          "id": "f5585432-df15-43de-bb9c-6f5207810bf6",
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
              "id": "28298f73-7fea-4224-a2a5-e2823d85d2d6"
            }
          ]
        },
        {
          "id": "79946462-fdd1-429e-8cce-5ee667473e75",
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
              "id": "47965ecb-d417-4192-8ab6-31d29895731a"
            }
          ]
        },
        {
          "id": "fdfc72ca-1753-4299-8127-2456aa812692",
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
              "id": "5c07fcb6-7bee-4402-b326-79320277ec9c"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "5d51a7f3-5172-4821-ba12-883c6cf43d7e",
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
              "id": "02a07600-fd4c-4b3b-aeb7-41286fec7900"
            }
          ]
        },
        {
          "id": "41e509c9-0a02-4ee3-883c-cc6b148293da",
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
              "id": "ade5bf61-061c-4454-99a7-9dad4c5c80f5"
            }
          ]
        },
        {
          "id": "aa87c5d9-75c8-4bc2-be43-f5287e91f55f",
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
              "id": "97399c1d-e643-488f-856b-47d6ffcc1af8"
            }
          ]
        },
        {
          "id": "9f52f86f-5448-48b8-812c-8a45af18a64b",
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
              "id": "533c0078-ebb8-44aa-ba79-c3de5409ff33"
            }
          ]
        },
        {
          "id": "1994f8d6-ec17-4362-8555-1586614f7cdf",
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
              "id": "5f38673b-c2d8-4248-ae2c-ac7f7565edf4"
            }
          ]
        },
        {
          "id": "e270cc6d-5d82-4380-8b59-9f3145b5a65d",
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
              "id": "b47b11a1-1a30-4871-b44f-fd56fb8c1a02"
            }
          ]
        },
        {
          "id": "ba12284c-39f8-42fd-a748-b89204ea7ba2",
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
              "id": "4d880eb5-3c33-4567-b63c-331664eccd98"
            }
          ]
        },
        {
          "id": "7d712586-9c2e-4394-bb10-88631413b65f",
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
              "id": "454feb6f-2d01-439b-ba25-92df0caa141a"
            }
          ]
        },
        {
          "id": "4e5c71e8-0c66-4aca-84b3-92bad2d473e4",
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
              "id": "4baaef13-1976-47a5-be5a-5af72deca4f1"
            }
          ]
        },
        {
          "id": "1baf7f4f-3569-4436-b1e7-cb227394c829",
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
              "id": "aeda94d7-98bc-4d66-ad00-8c8fe5077e61"
            }
          ]
        },
        {
          "id": "26696f46-4f9f-4442-bf10-6ca8530b7a7e",
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
              "id": "00299049-0bcf-4a0c-bcd6-33f6d9239fe0"
            }
          ]
        },
        {
          "id": "d5c8aa31-c605-4bad-b001-8147da625826",
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
              "id": "251e6801-02b3-4889-8e3a-4fb92e7102c9"
            }
          ]
        },
        {
          "id": "509f9d99-a032-4042-b743-9bef3ee93308",
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
              "id": "62665f19-c5d7-45fa-8589-7358496371c7"
            }
          ]
        },
        {
          "id": "fad0f8ce-b0f9-43f9-a10a-2b1ca74cc15b",
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
              "id": "906bb7b0-7021-4259-937c-5248932d9043"
            }
          ]
        },
        {
          "id": "29e631a3-9c4d-48b5-b514-d8961b7417f8",
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
              "id": "e27750d6-c6ba-4959-879a-d1620ec2bd3d"
            }
          ]
        },
        {
          "id": "93034992-b651-4e61-82cb-1a0093a1bf5f",
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
              "id": "19e038a5-276c-46ac-911b-9c3ce85cec3e"
            }
          ]
        },
        {
          "id": "2aa2540c-dc6c-4378-97fa-403a719d4895",
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
              "id": "eca54cc6-9e5b-4232-85e7-f08ea3cd29f5"
            }
          ]
        },
        {
          "id": "5d0cdea7-08db-4366-bd2d-9a66c966295b",
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
              "id": "dededc54-1f3a-4fbf-aa30-5e4f302453a2"
            }
          ]
        },
        {
          "id": "29ed9581-4e71-46d2-8062-580d443772fe",
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
              "id": "c6eb1acf-d16a-4737-b09e-4c95fc3dfb66"
            }
          ]
        },
        {
          "id": "23cdabb5-4581-4728-918f-a3a407f5d758",
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
              "id": "9b6caa3e-6d7c-48c4-9bbe-0ce7d3752862"
            }
          ]
        },
        {
          "id": "f155734d-7e4d-44eb-a46e-db6b809737fb",
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
              "id": "28989948-c58e-40f2-978f-09cbc3a6584b"
            }
          ]
        },
        {
          "id": "7f11cec1-7977-46e2-8a4e-a6d3b7feeffe",
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
              "id": "9038fbb7-e0e2-4795-b3c3-42dff627bbf3"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "40ccbddc-7de8-48ff-a5ea-f12c72e1e885",
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
              "id": "02a7db89-44f8-4593-9310-87b637855a34"
            }
          ]
        },
        {
          "id": "df9cd3f6-b1ec-4faa-a22a-675257589665",
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
              "id": "9f69a2bf-2e83-4bca-8662-3735a3d7a515"
            }
          ]
        },
        {
          "id": "384eae94-6b59-4cb4-a653-13997f81f152",
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
              "id": "148c12be-735b-47e0-a94d-7a001331e823"
            }
          ]
        },
        {
          "id": "f14e5cb5-36f3-4356-bfa0-70dbbe658f2b",
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
              "id": "e5b149b0-fa2b-4cdd-850d-fc4425208f1b"
            }
          ]
        },
        {
          "id": "724384be-7777-42f6-9315-5e7edefd5693",
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
              "id": "19c45c02-5dd5-40c0-b3a1-9b88091e126d"
            }
          ]
        },
        {
          "id": "0eb9f4c4-6f55-44d9-8e41-a31ad0f68314",
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
              "id": "bf0036cc-5b1f-40fc-b918-2536ccf84972"
            }
          ]
        },
        {
          "id": "9deef6cc-ba6b-4a37-a415-3ae82037c146",
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
              "id": "aa223ea9-101f-4e7f-8f64-d9032938e699"
            }
          ]
        },
        {
          "id": "2d1a54b6-9e0c-42dd-9df3-27412cd9972e",
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
              "id": "fe09c33e-7b99-4536-8377-3a79d9fdf6e8"
            }
          ]
        },
        {
          "id": "6b9c6222-a2b7-4960-93c7-03b1aba9b521",
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
              "id": "712eadd4-b93f-4478-8ab2-4bf80d765aa5"
            }
          ]
        },
        {
          "id": "6f13b5a4-4fad-43a9-bedb-1d24e3e66f6f",
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
              "id": "d4ed3dc6-dcba-4041-a411-1e4400bb31c0"
            }
          ]
        }
      ]
    },
    {
      "name": "ActiveDocs",
      "item": [
        {
          "id": "b56458f2-cb7a-4b50-b5c4-42057aa780e7",
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
              "id": "8ab0ada9-b5d4-4710-b8b0-1e5bb197734b"
            }
          ]
        }
      ]
    },
    {
      "name": "Limits",
      "item": [
        {
          "id": "aaf1d1b9-f6d9-4487-922c-2b1d3456452d",
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
              "id": "3b130280-2262-4f7a-b47b-bad5aafe692f"
            }
          ]
        }
      ]
    },
    {
      "name": "Limit",
      "item": [
        {
          "id": "f503afa0-4d8c-4379-9297-b32f50c1ea21",
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
              "id": "7ff03d32-37c1-4528-98de-85aea130466d"
            }
          ]
        },
        {
          "id": "d4913af6-374b-4eb4-9c72-c15e94c5657a",
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
              "id": "93b197b2-3bbf-4540-9f0c-ef1031b46bcf"
            }
          ]
        },
        {
          "id": "d88dcfe9-a6cf-48cc-81f9-c5bdab39509f",
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
              "id": "3d91174a-5305-45fa-93bb-333add761ca8"
            }
          ]
        },
        {
          "id": "fed7e2fc-b362-440f-a7cf-e6c8faf0e38a",
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
              "id": "8ca9dd79-9550-4b0f-a3c3-2cc4cd99357b"
            }
          ]
        },
        {
          "id": "8ec06266-ff92-463c-9611-3edda7c64aa8",
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
              "id": "b847ff76-637c-43d9-ae5b-fad5cef40d27"
            }
          ]
        },
        {
          "id": "060e8613-4f41-45af-a1ec-0a4ff48cab72",
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
              "id": "815824c8-c617-4bc2-925f-43984256b1c3"
            }
          ]
        },
        {
          "id": "1cd80e9c-39b8-4779-b0ff-a757ed4f3539",
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
              "id": "9765098c-ed6f-4708-9b34-42cb2bddf290"
            }
          ]
        },
        {
          "id": "adec12ca-e243-45b9-9cc7-893eea56f317",
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
              "id": "f33ec4d2-9f4e-4afb-973b-db58f16ee67c"
            }
          ]
        },
        {
          "id": "86f5cfea-47bf-4db2-995c-2d2d6766a278",
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
              "id": "f8e1bd86-4ef8-4d3e-889f-5821e6a7bebb"
            }
          ]
        },
        {
          "id": "fac6463a-7735-4aa4-ab3d-27e0e405c8bf",
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
              "id": "bb30bd0d-f0cb-4cad-a772-21970b3ae4f3"
            }
          ]
        }
      ]
    },
    {
      "name": "Pricing",
      "item": [
        {
          "id": "f724c760-6ab1-4f00-81b0-c57fc117343d",
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
              "id": "5649a333-0c01-42c4-9159-af36e58c019f"
            }
          ]
        },
        {
          "id": "1b3fa167-a452-44fc-ace6-9eaa0d657e1a",
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
              "id": "3f8da2c3-5b41-496e-bf76-46b96bec594d"
            }
          ]
        }
      ]
    },
    {
      "name": "End",
      "item": [
        {
          "id": "ffac2080-0b2b-48e7-8497-9f16d302a224",
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
              "id": "ff30cc8e-27fe-46ec-bb97-11773c1d5a7e"
            }
          ]
        }
      ]
    }
  ]
}