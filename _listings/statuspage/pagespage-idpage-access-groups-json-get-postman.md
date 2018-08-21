{
  "info": {
    "name": "StatusPage.io Retrieve a list of groups",
    "_postman_id": "563eac9e-e5c6-4d45-bf0b-48e6c89de771",
    "description": "Retrieve a list of groups",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pages",
      "item": [
        {
          "id": "94c4092c-128e-40cb-80e7-52359ef98b44",
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
              "id": "e7c2e7f3-254c-4b0e-97c0-db9b3d6c40bf"
            }
          ]
        },
        {
          "id": "78f5c1de-5888-41bd-82a4-702cb29b771b",
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
              "id": "8cbdaf1b-95e7-47c9-82b9-520b88236254"
            }
          ]
        }
      ]
    },
    {
      "name": "Components",
      "item": [
        {
          "id": "25da3e86-0447-4113-b8f5-5e20af0ca5d7",
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
              "id": "e6652fa9-6fa6-4394-854b-1bc51cff8f79"
            }
          ]
        },
        {
          "id": "f837f6a3-56df-4e78-bf96-e24a730af721",
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
              "id": "eeb9c4e8-8c5d-4a0f-80df-b83c5b7a6382"
            }
          ]
        },
        {
          "id": "e6f4123f-94bd-44bd-8249-761751a68913",
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
              "id": "7dae1148-59e4-4739-9022-c1b9c531cba3"
            }
          ]
        }
      ]
    },
    {
      "name": "Page Access Group",
      "item": [
        {
          "id": "fa43134b-235d-4804-a90c-53aaa3168510",
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
              "id": "5d28ea7b-4a02-4d15-bd71-ecb160499c44"
            }
          ]
        },
        {
          "id": "7b015e71-210b-48d3-8fb6-2c3665301418",
          "name": "retrieve-a-list-of-groups",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/page_access_groups.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a list of groups"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b034a00f-8739-4acf-b3e3-3c61a7997f4e"
            }
          ]
        }
      ]
    },
    {
      "name": "Incidents",
      "item": [
        {
          "id": "74dec586-3602-493f-ae4e-73305645bf26",
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
              "id": "df3eb2a9-9fde-457d-8bd0-b3143859fc85"
            }
          ]
        },
        {
          "id": "48cef438-f735-4818-80c5-0a09d25de2e3",
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
              "id": "52835a12-4a34-4fa0-a34d-3ad64204dfe7"
            }
          ]
        },
        {
          "id": "9ab21966-4e9e-498b-ad48-fc7fe4709e7d",
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
              "id": "3cf7eb6e-a710-4353-a808-cc578eaa7158"
            }
          ]
        },
        {
          "id": "540fef52-47a1-4660-bc35-42cafad5d126",
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
              "id": "9ba62ece-2939-48b4-b1d5-6eb2e9c8c933"
            }
          ]
        },
        {
          "id": "c9f4f7f5-3a99-49c9-93c6-ca8fc4c7c03a",
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
              "id": "dbe1d08c-1f5c-402d-9f5a-360a8798e11e"
            }
          ]
        },
        {
          "id": "26489ddc-fc0b-4cdd-abbd-5f910e9338fe",
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
              "id": "9e80899f-911e-4e70-8a5c-5dbdb32dda12"
            }
          ]
        },
        {
          "id": "72389eff-9347-4e7a-883b-595f6fbfb432",
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
              "id": "c5e57a69-670e-418b-8893-12d00f411e60"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscribers",
      "item": [
        {
          "id": "4fe26ad7-6147-46af-9054-ac881ee2cb84",
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
              "id": "b8d40d41-ed1e-4af0-9aaf-7104c9f6643d"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "bbe78e0f-6822-42a6-b75a-2e6286c086e5",
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
              "id": "86b0b5ce-4f04-455d-99d4-1ee07fc81437"
            }
          ]
        },
        {
          "id": "4cce6d8f-9cda-45ef-b96d-ce2cdccbd85c",
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
              "id": "0abacd39-5170-4de6-8024-afa81125a577"
            }
          ]
        },
        {
          "id": "44ab1a21-2430-41b7-9f6b-88ff97b4cadb",
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
              "id": "df264131-99ab-4f8c-8445-074d197e7555"
            }
          ]
        }
      ]
    },
    {
      "name": "Metric Providers",
      "item": [
        {
          "id": "42dce604-0d3b-40fb-9520-77818795b02b",
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
              "id": "a3cb717a-36cf-4436-b655-85d9d50ee5f3"
            }
          ]
        },
        {
          "id": "24becdf8-0e8c-4d62-a373-147482e435a2",
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
              "id": "7b6f2b0e-9d25-4507-9f30-63e939e1ee4f"
            }
          ]
        },
        {
          "id": "336f3b87-bd01-43eb-8793-371ba1036bb2",
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
              "id": "dde05b2b-a951-4661-9918-873eacdadcbc"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "7ad5e49b-2fcc-408c-9bf0-35bfda4ed492",
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
              "id": "1a95aef1-4b5e-4bb6-8530-3530d06188f2"
            }
          ]
        },
        {
          "id": "ced3edc0-200f-49ba-a19e-da27db70ca6f",
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
              "id": "e75aca7c-83d9-42be-a4ae-8df30aea9c36"
            }
          ]
        },
        {
          "id": "960f7b02-c83c-4a23-bb0e-e6955dd8792f",
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
              "id": "c224350b-2655-4b86-a991-36ee7b644a2b"
            }
          ]
        }
      ]
    },
    {
      "name": "Page Access Users",
      "item": [
        {
          "id": "0088f10b-fabb-494c-b70a-771c060f6835",
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
              "id": "22b53dce-c932-40c0-a164-0db8b8623b92"
            }
          ]
        },
        {
          "id": "60d57c44-61d4-49a4-8f08-f84ef908261b",
          "name": "create-a-user-who-can-view-your-status-page",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/page_access_users.json?page_access_user[component_ids=%5B%22page_access_user%5Bcomponent_ids%22%5D&page_access_user[email]=page_access_user%5Bemail%5D&page_access_user[external_login]=page_access_user%5Bexternal_login%5D&page_access_user[metric_ids=%5B%22page_access_user%5Bmetric_ids%22%5D&page_access_user[page_access_group_ids=%5B%22page_access_user%5Bpage_access_group_ids%22%5D&page_access_user[subscribe_to_components]=page_access_user%5Bsubscribe_to_components%5D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a user who can view your status page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5ec4dde-9421-4a58-b838-3cd80f4fc4be"
            }
          ]
        },
        {
          "id": "7fc07484-eb5b-42bd-b9e6-52e1b08b4814",
          "name": "delete-a-user-who-could-access-your-status-page",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/page_access_users/[page_access_user_id].json",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a user who could access your status page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29108641-84bd-4527-8c79-915d85e6a64f"
            }
          ]
        },
        {
          "id": "5eebab3f-c4ac-46e2-915f-b7547c2ec21b",
          "name": "change-information-for-a-user-who-can-view-your-status-page",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/page_access_users/[page_access_user_id].json?page_access_user[component_ids=%5B%22page_access_user%5Bcomponent_ids%22%5D&page_access_user[email]=page_access_user%5Bemail%5D&page_access_user[external_login]=page_access_user%5Bexternal_login%5D&page_access_user[metric_ids=%5B%22page_access_user%5Bmetric_ids%22%5D&page_access_user[page_access_group_ids=%5B%22page_access_user%5Bpage_access_group_ids%22%5D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Change information for a user who can view your status page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "456b1e33-dd01-4a0a-9513-032c001fb2fe"
            }
          ]
        },
        {
          "id": "d760aca5-ad0a-46bd-b179-63119d4bb4b9",
          "name": "assign-components-to-a-page-access-user-overwrites-existing-components",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/page_access_users/[page_access_user_id]/components.json?component_ids=%5B%22component_ids%22%5D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Assign components to a page access user (overwrites existing components)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d152855b-519d-4af0-83f8-1c804b0f781c"
            }
          ]
        },
        {
          "id": "5a03b0e1-8894-4b6f-8ad8-fe26aee56c4c",
          "name": "remove-all-components-from-a-page-access-user",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/page_access_users/[page_access_user_id]/components.json",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove all components from a page access user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b10c9564-55ac-43c2-bd6e-349b83bfd37c"
            }
          ]
        },
        {
          "id": "60d82793-b080-407a-9831-620c3b7cd08d",
          "name": "assign-components-to-a-page-access-user-adds-new-components-to-a-user",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/page_access_users/[page_access_user_id]/components.json?component_ids=%5B%22component_ids%22%5D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Assign components to a page access user (adds new components to a user)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f80f7555-0607-43f2-a5f5-72cd1a981204"
            }
          ]
        },
        {
          "id": "3cd73f38-b06a-4027-9cff-558e95f98201",
          "name": "assign-page-access-users-to-a-component",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/components/[component_id]/page_access_users.json?page_access_user_ids=%5B%22page_access_user_ids%22%5D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Assign page access users to a component"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e75467e-8df6-4445-a91e-0841b5cc6501"
            }
          ]
        },
        {
          "id": "9dbc2a05-e350-4c31-9caa-3e9c4160b474",
          "name": "remove-a-component-from-all-page-access-users",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/components/[component_id]/page_access_users.json",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a component from all page access users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd858ee2-a891-4ead-8bd3-85f2761f777a"
            }
          ]
        }
      ]
    }
  ]
}