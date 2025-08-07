![PyPI version](https://img.shields.io/pypi/v/graphql-schema-mcp.svg)
[![License](https://img.shields.io/github/license/hornedheck/graphql-schema-mcp.svg)](https://img.shields.io/github/license/hornedheck/graphql-schema-mcp/blob/main/LICENSE)
### Description

Working with large and complex GraphQL schema files can be challenging for AI agents due to context window limitations or the sheer size of the files.
This project provides a lightweight and efficient MCP server that enables search functionality over GraphQL schema files.

The server leverages vector search to create an indexed, searchable representation of the schema, allowing AI agents to perform fast and semantically relevant searches across GraphQL types.
It also supports MPS (Metal Performance Shaders) to accelerate embedding computations on Apple Silicon devices.

### Installation

#### Prerquisites:
- Python 3.12 or higher

#### Step 1: Install from PyPI:
```shell
pip3 install graphql-schema-mcp 
```
#### Step 2: Add to `mcp.json`
```json
    "GraphQLSchemaSearch": {
      "type" : "stdio",
      "command" : "graphql-schema-mcp"
    }
```