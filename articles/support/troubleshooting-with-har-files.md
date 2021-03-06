---
description: How to troubleshoot with HAR files and steps to generate a HAR file.
topics:
    - support
    - har-files
contentType:
  - how-to
  - reference
useCase:
  - support
---

# Troubleshooting with HAR files

Sometimes during development the authentication flow doesn't work as expected.

The fastest way to identify the underlying issue is to export a `HAR` file from Google Chrome Dev Tools. An **HTTP Archive (HAR) format** file, is a JSON formatted log file of all web browser interactions with web servers.

## Generating a HAR file:

1. Close all __incognito__ windows from Google Chrome.
1. Open a __new incognito__ tab on Google Chrome.
1. Open __Google Chrome Developers Tools__ on the new Incognito Window and click the Network Tab. Make sure you check the __Preserve Log__ options to record all interactions.
1. Proceed with the navigation that presents issues.
1. When complete, go back to the __Network__ tab, right click and then select **Save as HAR with Content**: ![Google Dev Tools](/media/articles/tutorials/save-as-har-with-content.png)
1. Before sending the HAR file to us, make sure to obfuscate any sensitive information using a text editor (such as remove passwords, client secrets, and so on).
1. Send the file to support by opening a [support ticket](${env.DOMAIN_URL_SUPPORT})
