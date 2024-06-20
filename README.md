# Product lifecycle & security API

## General 

The Product Lifecycle and Security API is a commercial service from Versio.io that allows you to verify the version characteristics, maintenance, support and security of your products and technologies in order to ensure IT governance. Please see [this link](https://www.versio.io/product-lifecycle-security-governance-api.html) for more!

In this GitHub repository, we give you guidance on trying out our REST API and integrating it into your environment.

A Swagger REST API documentation you found here: https://doc.versio.io/product-lifecycle-security-api/


## How you can use it

### Request API token

To try out the API, you need a personalized API token. You can request it here: https://www.versio.io/free-trial.html

### REST API client

The easiest way is to use the REST API via a REST API client. Below you can see an example REST API calls (see [rest-api-examples.http](rest-api-examples.http), please add your personal API token) with the Visual Code IDE:

![](https://www.versio.io/img/use-case/product-governance-api/versio.io-apache-tomcat-governance-check.gif)

Enclosed are the links for toolsetting:
1. Visual Code IDE: https://code.visualstudio.com/
1. REST Clint Plugin: https://marketplace.visualstudio.com/items?itemName=humao.rest-client

The following JSON represents the return result of an API call: 

```json
{
  "vendor": "Apache",
  "versioVendorLink": "https://live.versio.io/products?vendor=Apache",
  "product": "Tomcat",
  "versioProductLink": "https://live.versio.io/products?vendor=Apache&product=Tomcat",
  "version": "8.5.27",
  "vendorPublishedUtc": 1516306184000,
  "governanceRules": {
    "type": "Versio.io",
    "lifecycle": {
      "isStable": true,
      "isLatestRelease": false,
      "isLatestReleaseVersion": true,
      "isLatestLongTermSupportRelease": false,
      "isLongTermSupport": false,
      "hasSupport": false,
      "hasSupport_30d": false,
      "hasSupport_90d": false,
      "hasSupport_180d": false,
      "hasExtendedSupport": false,
      "hasExtendedSupport_30d": false,
      "hasExtendedSupport_90d": false,
      "hasExtendedSupport_180d": false,
      "hasMaintenance": true,
      "hasMaintenance_30d": false,
      "hasMaintenance_90d": false,
      "hasMaintenance_180d": false,
      "hasExtendedMaintenance": false,
      "hasExtendedMaintenance_30d": false,
      "hasExtendedMaintenance_90d": false,
      "hasExtendedMaintenance_180d": false
    },
    "security": {
      "noExplicitCves": true,
      "noAmbiguousCves": false,
      "noImplicitCves": false
    }
  },
  "governanceResults": {
    "lifecycle": {
      "result": false,
      "isStable": true,
      "isLatestRelease": false,
      "isLatestReleaseVersion": false,
      "isLatestLongTermSupportRelease": null,
      "isLongTermSupport": null,
      "hasSupport": null,
      "hasSupport_30d": null,
      "hasSupport_90d": null,
      "hasSupport_180d": null,
      "hasExtendedSupport": null,
      "hasExtendedSupport_30d": null,
      "hasExtendedSupport_90d": null,
      "hasExtendedSupport_180d": null,
      "hasMaintenance": null,
      "hasMaintenance_30d": null,
      "hasMaintenance_90d": null,
      "hasMaintenance_180d": null,
      "hasExtendedMaintenance": null,
      "hasExtendedMaintenance_30d": null,
      "hasExtendedMaintenance_90d": null,
      "hasExtendedMaintenance_180d": null
    },
    "security": {
      "result": false,
      "explicitCves": [
        {
          "name": "CVE-2018-8037",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2018-8037"
        },
        {
          "name": "CVE-2019-12418",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2019-12418"
        },
        {
          "name": "CVE-2019-17563",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2019-17563"
        },
        {
          "name": "CVE-2019-2684",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2019-2684"
        },
        {
          "name": "CVE-2020-11996",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2020-11996"
        },
        {
          "name": "CVE-2020-13934",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2020-13934"
        },
        {
          "name": "CVE-2020-13935",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2020-13935"
        },
        {
          "name": "CVE-2020-13943",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2020-13943"
        },
        {
          "name": "CVE-2020-17527",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2020-17527"
        },
        {
          "name": "CVE-2020-1935",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2020-1935"
        },
        {
          "name": "CVE-2020-1938",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2020-1938"
        },
        {
          "name": "CVE-2020-9484",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2020-9484"
        },
        {
          "name": "CVE-2021-24122",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2021-24122"
        },
        {
          "name": "CVE-2021-25122",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2021-25122"
        },
        {
          "name": "CVE-2021-25329",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2021-25329"
        },
        {
          "name": "CVE-2021-30640",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2021-30640"
        },
        {
          "name": "CVE-2021-33037",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2021-33037"
        },
        {
          "name": "CVE-2021-41079",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2021-41079"
        },
        {
          "name": "CVE-2021-43980",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2021-43980"
        },
        {
          "name": "CVE-2022-25762",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2022-25762"
        },
        {
          "name": "CVE-2022-42252",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2022-42252"
        },
        {
          "name": "CVE-2023-28708",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2023-28708"
        },
        {
          "name": "CVE-2024-21733",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2024-21733"
        }
      ],
      "ambiguousCves": [
        {
          "name": "CVE-2020-8022",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2020-8022"
        }
      ],
      "implicitCves": [
        {
          "name": "CVE-2016-5425",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2016-5425"
        },
        {
          "name": "CVE-2016-6325",
          "link": "https://live.versio.io/environmentSettings-cves?sourceId=CVE-2016-6325"
        }
      ]
    }
  },
  "recommendation": {
    "updateToVersion": [
      "9.0.90",
      "10.1.25"
    ]
  }
}
```

### Microsoft Excel

For all Microsoft Excel fans :-) we have provided a corresponding template with which you can use the REST API indirectly.

(see [versio.io-product-lifecycle-security-governance.xlsm](versio.io-product-lifecycle-security-governance.xlsm), please add your personal API token)


![](https://www.versio.io/img/use-case/product-governance-api/versio.io-product-compliance-ms-excel-integration-big.gif)


## User interface visualization

In the Versio.io user interface, we use this API to assess products and technologies for their lifecycle and security status:

![](https://www.versio.io/img/use-case/product-governance-api/versio.io-apache-tomcat-governance-check.png)

