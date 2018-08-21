{
  "info": {
    "name": "StatusPage.io Retrieve a list of users",
    "_postman_id": "478ac48d-ad7c-47ce-8f69-5cd9b5d38e4c",
    "description": "Retrieve a list of users",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pages",
      "item": [
        {
          "id": "35916bb3-02cd-48e8-ad7c-4125f0d2a48b",
          "name": "get-your-page-profile",
          "request": {
            "url": "http://example.com/api/pages/[page_id].json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get your page profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc8e3938-c5e5-47d2-bbbb-7c4bf4950d3b"
            }
          ]
        },
        {
          "id": "f6fa780e-2813-4cca-b76a-884e4dd1da8b",
          "name": "update-your-page-profile",
          "request": {
            "url": "http://example.com/api/pages/[page_id].json?basic layout only, 170x45 or 340x90 is best=basic%20layout%20only%2C%20170x45%20or%20340x90%20is%20best&page[allow_email_subscribers]=page%5Ballow_email_subscribers%5D&page[allow_incident_subscribers]=page%5Ballow_incident_subscribers%5D&page[allow_page_subscribers]=page%5Ballow_page_subscribers%5D&page[allow_sms_subscribers]=page%5Ballow_sms_subscribers%5D&page[city]=page%5Bcity%5D&page[country]=page%5Bcountry%5D&page[css_body_background_color]=page%5Bcss_body_background_color%5D&page[css_font_color]=page%5Bcss_font_color%5D&page[css_greens]=page%5Bcss_greens%5D&page[css_light_font_color]=page%5Bcss_light_font_color%5D&page[css_oranges]=page%5Bcss_oranges%5D&page[css_reds]=page%5Bcss_reds%5D&page[css_yellows]=page%5Bcss_yellows%5D&page[domain]=page%5Bdomain%5D&page[hero_cover_url]=page%5Bhero_cover_url%5D&page[layout]=page%5Blayout%5D&page[name]=page%5Bname%5D&page[notifications_from_email]=page%5Bnotifications_from_email%5D&page[state]=page%5Bstate%5D&page[subdomain]=page%5Bsubdomain%5D&page[time_zone]=page%5Btime_zone%5D&page[transactional_logo_url]=page%5Btransactional_logo_url%5D&page[url]=page%5Burl%5D&premium layout only, 850x315 or 1700x630 is best=premium%20layout%20only%2C%20850x315%20or%201700x630%20is%20best",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Update your page profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a03d0e9b-c2fe-4d91-a3ce-a9371a267a54"
            }
          ]
        }
      ]
    },
    {
      "name": "Components",
      "item": [
        {
          "id": "66045486-2650-4b07-8039-20887d3311d0",
          "name": "get-a-list-of-all-components",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/components.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of all components"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "597902b3-d410-4e0b-9e76-70ba866eb950"
            }
          ]
        },
        {
          "id": "35e4c5f9-c65e-45c2-94c0-846509752cf7",
          "name": "create-a-component",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/components.json?component[description]=component%5Bdescription%5D&component[group_id]=component%5Bgroup_id%5D&component[name]=component%5Bname%5D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a component"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b4697e4-60f9-4c4f-b744-351266f20265"
            }
          ]
        },
        {
          "id": "df09e310-326e-4a4b-9699-d0aeea5c63f7",
          "name": "delete-a-component",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/components/[component_id].json",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a component"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ccd4aca-cdf8-4938-bebb-1aa54ae53b81"
            }
          ]
        }
      ]
    },
    {
      "name": "Page Access Group",
      "item": [
        {
          "id": "9c1b0dfe-4140-4460-b130-0fd5cde8a2a6",
          "name": "update-a-component",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/components/[component_id].json?component[description]=component%5Bdescription%5D&component[name]=component%5Bname%5D&component[status]=component%5Bstatus%5D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Update a component"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd03ed10-8f6f-4ffd-8e57-2a329c93def5"
            }
          ]
        }
      ]
    },
    {
      "name": "Incidents",
      "item": [
        {
          "id": "f61cfa64-6042-4245-b807-2d2f0c238882",
          "name": "get-a-list-of-all-incidents",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of all incidents"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a798fa7-5c3f-4e60-8dd6-f8295bb106ff"
            }
          ]
        },
        {
          "id": "7ca300b5-e7dc-451a-9101-26de460d69af",
          "name": "create-a-realtime-incident",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents.json?incident[backfilled]=incident%5Bbackfilled%5D&incident[backfill_date]=incident%5Bbackfill_date%5D&incident[component_ids]=incident%5Bcomponent_ids%5D&incident[impact_override]=incident%5Bimpact_override%5D&incident[message]=incident%5Bmessage%5D&incident[name]=incident%5Bname%5D&incident[scheduled_auto_completed]=incident%5Bscheduled_auto_completed%5D&incident[scheduled_auto_in_progress]=incident%5Bscheduled_auto_in_progress%5D&incident[scheduled_for]=incident%5Bscheduled_for%5D&incident[scheduled_remind_prior]=incident%5Bscheduled_remind_prior%5D&incident[scheduled_until]=incident%5Bscheduled_until%5D&incident[status]=incident%5Bstatus%5D&incident[wants_twitter_update]=incident%5Bwants_twitter_update%5D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a realtime incident"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0845b071-6089-4c68-86fa-e9d5273406f3"
            }
          ]
        },
        {
          "id": "38f1973f-765e-4d90-9f45-d601049f97bf",
          "name": "unresolved-only",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents/unresolved.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Unresolved Only"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00a64f16-129e-4c1a-977e-2dcf86a75d10"
            }
          ]
        },
        {
          "id": "0fab4a89-65ce-4931-85c2-499e4ae2fb0e",
          "name": "scheduled-only",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents/scheduled.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Scheduled Only"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55420b13-e750-432b-a1e9-21f4865c4910"
            }
          ]
        },
        {
          "id": "1270d7f5-b97f-4e2a-91e6-19c296c75211",
          "name": "delete-an-incident",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents/[incident_id].json",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an incident"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4ff4517-cf56-49f8-a6ee-aeb9c9321071"
            }
          ]
        },
        {
          "id": "58c3224c-f1a0-4ca6-a59b-6c02594511ad",
          "name": "update-an-incident-only-applies-to-realtime-and-scheduled-incidents",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents/[incident_id].json?at the same time to avoid two separate incident updates being generated.=at%20the%20same%20time%20to%20avoid%20two%20separate%20incident%20updates%20being%20generated.&ENDPOINT=ENDPOINT&incident[component_ids]=incident%5Bcomponent_ids%5D&incident[impact_override]=incident%5Bimpact_override%5D&incident[message]=incident%5Bmessage%5D&incident[name]=incident%5Bname%5D&incident[status]=incident%5Bstatus%5D&incident[wants_twitter_update]=incident%5Bwants_twitter_update%5D&MUTABLE=MUTABLE&PATCH /pages/[page_id]/incidents/[incident_id].json=PATCH%20%2Fpages%2F%5Bpage_id%5D%2Fincidents%2F%5Bincident_id%5D.json",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Update an incident (only applies to realtime and scheduled incidents)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37237eff-7204-40a3-baa9-41405d179f8d"
            }
          ]
        },
        {
          "id": "8210b337-ec1e-45c0-b6d9-bc1e75958289",
          "name": "tune-an-incident-update",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/incidents/[incident_id]/incident_updates/[incident_update_id].json?incident_update[body]=incident_update%5Bbody%5D&incident_update[display_at]=incident_update%5Bdisplay_at%5D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Tune an Incident Update"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "039caa3b-01aa-43fd-bc46-68a81795af6b"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscribers",
      "item": [
        {
          "id": "a945b001-6cf1-48db-ba61-1edd5ca0596e",
          "name": "delete-a-subscriber",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/subscribers/[subscriber_id].json",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a subscriber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2240b3c4-bcc7-4916-aacf-f5b3c64d4cda"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "903f250b-fb16-440d-9095-92d7cd76adf4",
          "name": "get-a-list-of-available-public-metric-providers",
          "request": {
            "url": "http://example.com/api/metrics_providers.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of available public metric providers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6055861f-5f8b-4400-b4b1-2f41d8b1a106"
            }
          ]
        },
        {
          "id": "6cc44ce5-10d4-4a61-9340-e91b08a9a202",
          "name": "submit-data-for-a-custom-metric",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/metrics/[metric_id]/data.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Submit data for a custom metric"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f582784-440d-47ad-bbbb-74051c03bb6d"
            }
          ]
        },
        {
          "id": "171bf74c-55f5-4ff2-a8bc-3131172ba903",
          "name": "delete-all-data-for-a-custom-metric",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/metrics/[metric_id]/data.json",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete all data for a custom metric"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3ee3927-eb19-4171-94b6-dd5962938702"
            }
          ]
        }
      ]
    },
    {
      "name": "Metric Providers",
      "item": [
        {
          "id": "ae0472d3-879f-42af-9f03-f2b4f301e65d",
          "name": "get-a-list-of-metric-providers-linked-to-your-page",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/metrics_providers.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of metric providers linked to your page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c5c6228-81bd-4b47-96dd-621cc4e9a7ec"
            }
          ]
        },
        {
          "id": "bccc8ead-df24-4ae5-ae77-06e1a60969ad",
          "name": "get-a-list-of-metrics-created-for-a-linked-metrics-provider",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/metrics_providers/[metrics_provider_id]/metrics.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of metrics created for a linked metrics provider"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f06e6e9a-01ea-44f1-b0e7-57a9b6d51b99"
            }
          ]
        },
        {
          "id": "5ddbc7b8-e5a4-423e-a783-775babf9ca6e",
          "name": "create-a-custom-metric",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/metrics_providers/[metrics_provider_id]/metrics.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a custom metric"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "670f520e-8f77-4fb5-a404-0b17f3bad6f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "96b0d570-5398-470d-ae72-b0a9494e9603",
          "name": "list-users",
          "request": {
            "url": "http://example.com/api/organizations/[organization_id]/users.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8abc3d2-fe19-41ee-9b04-2c6826ee19b0"
            }
          ]
        },
        {
          "id": "ca040d11-16e9-4910-ad59-b28a6036ead2",
          "name": "create-a-user",
          "request": {
            "url": "http://example.com/api/organizations/[organization_id]/users.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb490179-990e-419c-853a-8253315da957"
            }
          ]
        },
        {
          "id": "75b3575f-54ee-4ccf-927b-89544ae730a4",
          "name": "delete-a-user",
          "request": {
            "url": "http://example.com/api/organizations/[organization_id]/users/[user_id].json",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d33b2aa9-3a44-482b-a0e9-2acb7921a080"
            }
          ]
        }
      ]
    },
    {
      "name": "Page Access Users",
      "item": [
        {
          "id": "c090f459-9d73-4c7f-8436-cc0cabc7d89b",
          "name": "retrieve-a-list-of-users",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/page_access_users.json?email=email",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a list of users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4475d3a-73ea-4734-872c-be9bf7c3a42f"
            }
          ]
        }
      ]
    }
  ]
}