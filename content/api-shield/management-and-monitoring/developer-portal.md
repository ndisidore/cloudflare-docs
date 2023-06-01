---
pcx_content_type: how-to
type: overview
title: Build developer portals
weight: 3
---

# Build developer portals

Once endpoints are saved into Endpoint Management, API Shield doubles as an API catalog. API Shield can build an interactive documentation portal with the knowledge it has of your APIs, or you can upload a new OpenAPI schema file to build a documentation portal ad-hoc.

## Process

1. Log in to the [Cloudflare dashboard](https://dash.cloudflare.com/) and select your account and domain.
2. Go to **Security** > **API Shield** > **Settings**.
3. Under **Create a developer portal**, select **Create site**.
4. Upload an OpenAPI v3.0 schema file or choose to select an existing schema from API Shield. 

    {{<Aside type="note">}} 
If you do not have a schema to upload or to select from a pre-existing schema, export your Endpoint Management schema. For best results, include the learned parameters. 

Only API schemas uploaded to Schema Validation 2.0 are available when selecting existing schemas
    {{</Aside>}}

5. Select **Download project files** to save a local copy of the files that will be uploaded to Cloudflare Pages. Downloading the project files can be helpful if you wish to modify the project in any way and then upload the new version manually to Pages.
6. Select **Create pages project** to begin project creation. A new Pages project will be automatically created and your API schema will be automatically uploaded to the project along with other supporting static content.
7. Select **Deploy site**. 

### Custom domains

To create a vanity domain instead of using the pages.dev domain, refer to the [Pages custom domain documentation](/pages/platform/custom-domains/).

## Availability

Building developer portals is available to all API Shield subscribers. This feature uses Cloudflare Pages to host the resulting portal. Refer to [Pages](/pages/) for any limitations of your current subscription plan.

## Limitations

This feature currently uses the open source [Redoc](https://github.com/Redocly/redoc) project from [Redocly](https://redocly.com/). For custom theme and branding options, visit the [Redoc GitHub repository](https://github.com/Redocly/redoc). 

To modify the resulting page, download the project files before creating the Pages project. You can create a new Pages project with the modified files you have made to meet your branding guidelines.