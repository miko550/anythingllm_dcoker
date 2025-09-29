# anythingllm_docker
Docker Compose for anythingllm deployment

# Setup
```
git clone https://github.com/miko550/anythingllm_docker.git
cd anythingllm_docker
docker compose up -d
```

# add MCP for docker-mcp-gateywat
1.Edit
`nano ./data/plugins/anythingllm_mcp_servers.json`
3. add mcp
```
{
  "mcpServers": {
    "docker-mcp-gateway": {
      "type": "streamable",          // or "sse" if you set --transport=sse
      "url": "http://gateway:8811/mcp"
    }
  }
}
```

