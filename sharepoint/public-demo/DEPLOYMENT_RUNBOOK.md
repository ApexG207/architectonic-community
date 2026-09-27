# Architectonic Public Demo SharePoint Deployment Runbook v0.1

## Preconditions
1. Confirm the target SharePoint tenant/site allows the intended external/public audience.
2. Confirm only synthetic or cleared public content will be loaded.
3. Confirm no public/anonymous sharing is enabled unless separately authorized by the tenant owner.
4. Confirm site owner and demo reviewer.
5. Establish TEST before public publication.

## Deployment sequence
1. Create or approve the site: Architectonic Community Demo.
2. Create demo libraries defined in SHAREPOINT_PUBLIC_DEMO_ARCHITECTURE.md.
3. Create site columns from site_columns.json.
4. Create content types from content_types.json.
5. Create Lists from lists.json.
6. Apply versioning and public-demo metadata controls.
7. Map approved roles using permissions_matrix.csv.
8. Implement Power Automate flows in TEST.
9. Connect Power BI to demo lists using powerbi_model.json.
10. Load the Northstar synthetic scenario and other approved public artifacts.
11. Run public-boundary tests.
12. Obtain demo publication approval.
13. Publish only the explicitly accepted demo surface.

## Minimum acceptance tests
- all demo pilot records have Synthetic_Flag=true;
- demo site contains no client data or nonpublic government data;
- demo contributors cannot alter Enterprise records;
- demo content contains no private prompt/orchestration library;
- publication review blocks unreviewed content;
- public/private boundary page is visible;
- all dashboards state synthetic/demo status;
- no production connector secrets or internal URLs are exposed.

## Rollback
- unpublish affected pages/content;
- disable demo flows;
- revoke external sharing if enabled;
- restore prior file versions where supported;
- preserve review evidence;
- correct boundary violations before republishing.

## Deployment status
NOT LIVE-DEPLOYED by this package. Actual hostname, site path, sharing model, identities, and tenant policy remain unresolved until a specific environment is selected.
