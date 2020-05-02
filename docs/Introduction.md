# Introduction

Welcome to the Dataflow Kit (DFK) API! 

DFK’s API enables you to programatically manage and run your web data extraction and SERPs collection Tasks. You can easily retrieve extracted data afterwards. 

Rendering web pages, Converting URLs to PDF or Capturing a web page screenshots are also can be run in Dataflow kit cloud.

Quick links to DFK API services:

- [Extract web data](#extract-data-from-web)
- [Scrape search engine results (SERPs)](#extract-serps) 
- [Render JS Dynamic HTML pages](#fetch-html)  
- [Capture a screenshot](#capture-a-screenshot)
- [Convert URL to PDF](#convert-url-to-pdf)

Curl, Go, Python, Node.js, and PHP code examples are available. You can view them in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right. By default, curl is selected so that you can try out the commands in your terminal.

## Authentication

> To authorize, use this code:

```shell
# With shell, you can just pass a valid API Key with each request
curl --request POST \
     --url https://api.dataflowkit.com/v1/{API-ENDPOINT}?api_key=YOUR_API_KEY -d \
'{
  "foo":"bar"
}'
```

>API-ENDPOINT corresponds to specified API endpoint. 
>Make sure to replace `YOUR_API_KEY` with your API key.

After signing up, every user is assigned a personal API Access Key - a unique "password" used to make requests to the Dataflow Kit API.

Dataflow Kit API needs to be authenticated by passing a secret API Key to all API requests to the server as the <code>api_key</code> query parameter. 

It looks like the following: 
`api_key=YOUR_API_KEY`

The API Key can be found in the [DFK Dashboard](https://account.dataflowkit.com) after registration. 

Once you sign-up, we grant you free 1000 credits which is equal to €5 for evaluation and testing.

<aside class="success">
You must replace <code>YOUR_API_KEY</code> with your personal API key.
</aside>

<aside class="warning">
IMPORTANT: Do not share the API Key with untrusted parties, or use it directly from a client-side code, unless you fully understand the consequences!
</aside>

## Versioning
All Dataflow Kit API endpoints URLs start with https://api.dataflowkit.com/v1/.

The current API version 1 is available via the /v1 prefix. 

If there are backward incompatible changes that need to be made to our API, we will release a new API version. The previous API version will be maintained for at least a year after releasing the new version.



