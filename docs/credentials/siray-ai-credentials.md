# Siray AI credentials

You can use these credentials to authenticate the following nodes:

- Siray Chat
- Siray Embedding
- Siray Image
- Siray Video
- Siray Image Trigger
- Siray Video Trigger

## Prerequisites

- Create a Siray AI account.

## Supported authentication methods

- API key

## Related resources

- Refer to Siray AI's API documentation for more information about the service.

## Using API key

To configure this credential, you'll need:

- An API key
- (Optional) Base URL — defaults to `https://api.siray.ai` if your workspace doesn't specify a custom endpoint.

To generate your API key:

1) Log in to your Siray AI account and open the **API keys** section in the dashboard.
2) Select **Create new secret key** (or similar) to create a key, optionally naming it for the environment.
3) Copy the key and add it as the **API Key** value in n8n.

If your Siray deployment uses a custom domain, set that value as the **Base URL**; otherwise leave the default.
