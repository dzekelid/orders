---
name: Xero
x-slug: xero
description: Xero is the QuickBooks alternative. Use Xero accounting software to manage
  invoicing, bank reconciliation, bookkeeping & more. Start a free trial today!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
x-kinRank: "8"
x-alexaRank: "2158"
tags: Orders
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/xero/apis.md
specificationVersion: "0.14"
apis:
- name: Clarity Accounting Get Purchaseorders
  x-api-slug: clarity-accounting
  description: Get purchaseorders.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//PurchaseOrders
  tags: PurchaseOrders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/xero/purchaseorders-get-openapi.md
- name: Clarity Accounting Post Purchaseorders
  x-api-slug: clarity-accounting
  description: Post purchaseorders.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//PurchaseOrders
  tags: PurchaseOrders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/xero/purchaseorders-post-openapi.md
- name: Clarity Accounting Put Purchaseorders
  x-api-slug: clarity-accounting
  description: Put purchaseorders.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//PurchaseOrders
  tags: PurchaseOrders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/xero/purchaseorders-put-openapi.md
- name: Clarity Accounting X-related-model Purchaseorders
  x-api-slug: clarity-accounting
  description: X-related-model purchaseorders.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//PurchaseOrders
  tags: PurchaseOrders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/xero/purchaseorders-xrelatedmodel-openapi.md
- name: Clarity Accounting Get Purchaseorders Purchaseorder
  x-api-slug: clarity-accounting
  description: Get purchaseorders purchaseorder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//PurchaseOrders/{PurchaseOrderID}
  tags: PurchaseOrders,PurchaseOrderID
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/xero/purchaseorderspurchaseorderid-get-openapi.md
- name: Clarity Accounting Post Purchaseorders Purchaseorder
  x-api-slug: clarity-accounting
  description: Post purchaseorders purchaseorder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//PurchaseOrders/{PurchaseOrderID}
  tags: PurchaseOrders,PurchaseOrderID
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/xero/purchaseorderspurchaseorderid-post-openapi.md
- name: Clarity Accounting X-related-model Purchaseorders Purchaseorder
  x-api-slug: clarity-accounting
  description: X-related-model purchaseorders purchaseorder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//PurchaseOrders/{PurchaseOrderID}
  tags: PurchaseOrders,PurchaseOrderID
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/xero/purchaseorderspurchaseorderid-xrelatedmodel-openapi.md
- name: Clarity Accounting Get Purchaseorders Purchaseorder Attachments
  x-api-slug: clarity-accounting
  description: Get purchaseorders purchaseorder attachments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//PurchaseOrders/{PurchaseOrderID}/Attachments
  tags: PurchaseOrders,PurchaseOrderID,Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/xero/purchaseorderspurchaseorderidattachments-get-openapi.md
- name: Clarity Accounting Get Purchaseorders Purchaseorder Attachments Filename
  x-api-slug: clarity-accounting
  description: Get purchaseorders purchaseorder attachments filename.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//PurchaseOrders/{PurchaseOrderID}/Attachments/{FileName}
  tags: PurchaseOrders,PurchaseOrderID,Attachments,FileName
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/xero/purchaseorderspurchaseorderidattachmentsfilename-get-openapi.md
- name: Clarity Accounting Post Purchaseorders Purchaseorder Attachments Filename
  x-api-slug: clarity-accounting
  description: Post purchaseorders purchaseorder attachments filename.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//PurchaseOrders/{PurchaseOrderID}/Attachments/{FileName}
  tags: PurchaseOrders,PurchaseOrderID,Attachments,FileName
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/xero/purchaseorderspurchaseorderidattachmentsfilename-post-openapi.md
- name: Clarity Accounting
  x-api-slug: clarity-accounting
  description: Xero is the QuickBooks alternative. Use Xero accounting software to
    manage invoicing, bank reconciliation, bookkeeping & more. Start a free trial
    today!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0
  tags: Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/xero/openapi.md
x-common:
- type: x-base
  url: https://api.xero.com
- type: x-blog
  url: http://blog.xero.com
- type: x-blog
  url: https://devblog.xero.com/
- type: x-blog-rss
  url: https://devblog.xero.com/feed
- type: x-blog-rss
  url: http://feeds.feedburner.com/xerolive
- type: x-crunchbase
  url: http://www.crunchbase.com/company/xero
- type: x-crunchbase
  url: https://crunchbase.com/organization/xero
- type: x-developer
  url: http://developer.xero.com/
- type: x-email
  url: support@xero.com
- type: x-email
  url: sales@xero.com
- type: x-email
  url: careers@xero.com
- type: x-email
  url: privacy@xero.com
- type: x-email
  url: phishing@xero.com
- type: x-email
  url: press@xero.com
- type: x-email
  url: AUpress@xero.com
- type: x-email
  url: UKpress@xero.com
- type: x-email
  url: USpress@xero.com
- type: x-github
  url: https://github.com/XeroAPI
- type: x-partners
  url: http://developer.xero.com/partner/
- type: x-pricing
  url: https://www.xero.com/us/pricing/
- type: x-twitter
  url: https://twitter.com/xero
- type: x-website
  url: http://www.xero.com/
- type: x-website
  url: http://xero.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---