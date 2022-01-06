---
title: "Mendix Runtime"
url: /refguide7/runtime/
---

## 1 Introduction

The Mendix Runtime executes the application model that is created in the Modeler. It serves pages to the Mendix Client, executes microflows, calls web services, generates documents, communicates with the database, and much more.

## 2 Licensing

You need a license to run an application in production mode. Without a license, the Mendix Runtime stops operating after a couple of hours. A license can be obtained through your account manager at Mendix. Afterwards, you can activate your license by following the instructions in [How to Activate Your Mendix License on Microsoft Windows](/developerportal/deploy/activate-a-mendix-license-on-microsoft-windows/).

## 3 APIs

You can extend the functionality of the Runtime by writing Java actions. For more information,  see the [Runtime API](/apidocs-mxsdk/apidocs/#runtime) section of *API Documentation*.

{{% alert type="info" %}}
Links to available API documentation such as WSDLs for published web services are available on the URL path `/api-doc` (for example: `http://localhost:8080/api-doc/`).
{{% /alert %}}

## 4 Main Documents in This Category

* [Clustered Mendix Runtime](/refguide/clustered-mendix-runtime/)
* [Customization](/refguide/custom-settings/)
* [Data Storage](/refguide/data-storage/)
* [Date & Time Handling](/refguide/datetime-handling-faq/)
* [Logging](/refguide/logging/)
* [Monitoring Mendix Runtime](/refguide/monitoring-mendix-runtime/)
* [Objects & Caching](/refguide/objects-and-caching/)
* [Transient Objects & Garbage Collecting](/refguide/transient-objects-garbage-collecting/)
