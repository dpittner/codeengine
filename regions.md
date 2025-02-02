---

copyright:
  years: 2023
lastupdated: "2023-06-13"

keywords: regions for code engine, target region for code engine, endpoints for code engine, api endpoints in code engine, regions, endpoints

subcollection: codeengine

---

{{site.data.keyword.attribute-definition-list}}

# Regions 
{: #regions}

{{site.data.keyword.codeenginefull}} is available in the following regions:
{: shortdesc}

- Americas: Sao Paulo, Brazil (`br-sao`) region
- Americas: Toronto, Canada (`ca-tor`) region
- Americas: US East (`us-east`) region
- Americas: US South (`us-south`) region
- Asia Pacific: Sydney, Australia  (`au-syd`) region
- Asia Pacific: Osaka, Japan  (`jp-osa`) region
- Asia Pacific: Tokyo, Japan  (`jp-tok`) region
- Europe: Germany (`eu-de`) region
- Europe: Great Britain (`eu-gb`) region

You can target a specific region whenever you log in to the {{site.data.keyword.cloud_notm}} CLI or change your current region by using the [`target -r`](/docs/cli?topic=cli-ibmcloud_cli#ibmcloud_target) option.


```txt
ibmcloud target -r <region>
```
{: pre}

For example, to target the US South region:

```txt
ibmcloud target -r us-south
```
{: pre}

## {{site.data.keyword.codeengineshort}} endpoints for managing project resources
{: #endpoints-project}

Use the following endpoints to access and manage project resources.

| Region | Public endpoint | Private endpoint |
| ---- | -------- | -------- |
| Americas: Sao Paulo, Brazil | `api.br-sao.codeengine.cloud.ibm.com` | `api.private.br-sao.codeengine.cloud.ibm.com` |
| Americas: Toronto, Canada | `api.ca-tor.codeengine.cloud.ibm.com` | `api.private.ca-tor.codeengine.cloud.ibm.com` |
| Americas: US East | `api.us-east.codeengine.cloud.ibm.com` | `api.private.us-east.codeengine.cloud.ibm.com` |
| Americas: US South | `api.us-south.codeengine.cloud.ibm.com` | `api.private.us-south.codeengine.cloud.ibm.com` |
| Asia Pacific: Sydney, Australia | `api.au-syd.codeengine.cloud.ibm.com` | `api.private.au-syd.codeengine.cloud.ibm.com` |
| Asia Pacific: Osaka, Japan | `api.jp-osa.codeengine.cloud.ibm.com` | `api.private.jp-osa.codeengine.cloud.ibm.com` |
| Asia Pacific: Tokyo, Japan | `api.jp-tok.codeengine.cloud.ibm.com` | `api.private.jp-tok.codeengine.cloud.ibm.com` |
| Europe: Germany | `api.eu-de.codeengine.cloud.ibm.com` | `api.private.eu-de.codeengine.cloud.ibm.com` |
| Europe: Great Britain | `api.eu-gb.codeengine.cloud.ibm.com` | `api.private.eu-gb.codeengine.cloud.ibm.com` |
{: caption="{{site.data.keyword.codeengineshort}} endpoints for project resources" caption-side="bottom"}

## {{site.data.keyword.codeengineshort}} endpoints for accessing applications
{: #endpoints-app}

Use the following endpoints to access applications. 

The default URL for applications is of the format `https://<appname>.<uuid>.<region>.codeengine.appdomain.cloud` where `appname` is the name of your app, `uuid` is the automatically generated unique identifier, and `region` is the region in which your {{site.data.keyword.codeengineshort}} project resides. The UUID portion of the URL of an application is of the format `aaaabbbbccc`. The automatically generated application URL persists for the lifecycle of the project for your application. 




| Region | Public endpoint | Private endpoint |
| ---- | -------- | -------- |
| Americas: Sao Paulo, Brazil  | `app.uuid.br-sao.codeengine.appdomain.cloud` | `app.uuid.private.br-sao.codeengine.appdomain.cloud` |
| Americas: Toronto, Canada | `app.uuid.ca-tor.codeengine.appdomain.cloud` | `app.uuid.private.ca-tor.codeengine.appdomain.cloud` |
| Americas: US East | `app.uuid.us-east.codeengine.appdomain.cloud` | `app.uuid.private.us-east.codeengine.appdomain.cloud` |
| Americas: US South| `app.uuid.us-south.codeengine.appdomain.cloud` | `app.uuid.private.us-south.codeengine.appdomain.cloud` |
| Asia Pacific: Sydney, Australia  | `app.uuid.au-syd.codeengine.appdomain.cloud` | `app.uuid.private.au-syd.codeengine.appdomain.cloud` |
| Asia Pacific: Osaka, Japan | `app.uuid.jp-osa.codeengine.appdomain.cloud` | `app.uuid.private.jp-osa.codeengine.appdomain.cloud` |
| Asia Pacific: Tokyo, Japan | `app.uuid.jp-tok.codeengine.appdomain.cloud` | `app.uuid.private.jp-tok.codeengine.appdomain.cloud` |
| Europe: Germany | `app.uuid.eu-de.codeengine.appdomain.cloud` | `app.uuid.private.eu-de.codeengine.appdomain.cloud` |
| Europe: Great Britain | `app.uuid.eu-gb.codeengine.appdomain.cloud` | `app.uuid.private.eu-gb.codeengine.appdomain.cloud` |
{: caption="{{site.data.keyword.codeengineshort}} endpoints for apps" caption-side="bottom"}


