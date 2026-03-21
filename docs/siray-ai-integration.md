# Siray AI node

Use the Siray AI nodes to automate tasks with Siray's chat, embedding, image, and video models. The integration provides built-in operations for common generation workflows and can connect Siray to other applications in n8n.

On this page, you'll find the operations each Siray node supports and links to related resources.


## Credentials

Refer to [Siray AI credentials](/docs/siray-ai-credentials.md) for guidance on setting up authentication.

## Operations

**Text**
- Generate a Chat Completion

**Embeddings**
- Create an Embedding

**Image**
- Generate an Image (text-to-image or image-to-image)

**Video**
- Generate a Video (text-to-video or image-to-video)


## Related resources

- Siray AI API documentation: https://docs.siray.ai

## What to do if your operation isn't supported

If the available nodes don't cover your use case, use the HTTP Request node to call Siray's REST API directly:
- In the HTTP Request node, select `Authentication > Predefined Credential Type`.
- Choose `Siray API` and select your credential.
- Build the request for the desired Siray endpoint.

## Using tools with Siray

The Siray nodes are marked as usable tools, so you can connect them with the Tools connector when orchestrating agent-style workflows.

Operations that support tool connectors:
- Text: Generate a Chat Completion
- Image: Generate an Image
- Video: Generate a Video

## Common issues

- **Authentication errors:** Confirm the API key is valid and the Base URL matches your Siray deployment (defaults to `https://api.siray.ai`).
- **Model not found:** Pick a model exposed by your workspace; see `SirayModel.ts` for the bundled options.
- **Long-running generations:** Image and video requests are asynchronous; handle task IDs and polling as needed in your workflow.
