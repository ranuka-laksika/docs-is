The [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) provides a standardized way for AI agents and applications to interact with model resources. {{ product_name }} offers capabilities to control these interactions, ensuring that access to MCP servers and their resources is secure and well-managed.

## [Securing MCP servers]({{base_path}}/guides/agentic-ai/mcp/mcp-server-authorization)

MCP servers can be registered as protected resources in {{ product_name }}. This setup allows administrators to define precise access controls for each server and their tools and resources, specifying which clients or users are authorized to interact with it. By securely exposing remote MCP servers, organizations can maintain consistent authorization rules and minimize the risk of unauthorized access to MCP servers and their tools, and protect underlying business resources.

## [Setting up MCP clients]({{base_path}}/guides/agentic-ai/mcp/register-mcp-client-app)

An MCP client is a connection component that host applications use to interface with MCP servers through dedicated, stateful sessions. {{ product_name }} supports MCP server authorization for all OIDC application types, including Custom OIDC applications, Traditional Web applications, Single-Page applications (SPA), Mobile applications, and Machine-to-Machine (M2M) applications. 

The [MCP client Application template]({{base_path}}/guides/agentic-ai/mcp/register-mcp-client-app) provides a pre-configured option optimized for MCP-specific use cases, creating an OAuth 2.1 client that meets the necessary standards. However, any OIDC application can be authorized to access MCP servers. Applications can be authorized with specific scopes that define their permitted access to MCP servers, ensuring they operate only within authorized boundaries and maintain a secure ecosystem for model interactions.

!!! note
    Digital Wallet applications have an Authorization tab but can only access Verifiable Credential resources. They cannot authorize MCP servers.

Through these features, {{ product_name }} centralizes the management of MCP authorization, making it easier to enforce secure interactions between clients and servers, maintain compliance, and manage permissions efficiently across AI agent ecosystems.
