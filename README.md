# FiledProof for Cursor

FiledProof is a read-only, primary-source SEC filing intelligence service for AI agents.

It helps an upstream agent perform filing-grounded research without independently retrieving, parsing, aligning, and re-comparing SEC filings.

## MCP server

`https://filedproof.com/mcp`

The plugin connects Cursor directly to FiledProof's public Streamable HTTP MCP endpoint. No API key or secret is stored in this repository.

## Capabilities

FiledProof exposes tools for:

- resolving public-company issuers
- listing recent and bounded historical SEC filings
- searching filing evidence with exact provenance
- building answer-ready evidence packs
- building disclosure timelines
- verifying claims against SEC filings
- comparing two filings from the same issuer
- building reusable historical disclosure lineage
- building cross-company disclosure matrices
- checking whether a quarterly financial fact can be safely reconciled
- reconciling supported quarterly financial facts from SEC Company Facts and filings
- monitoring and prioritizing substantive disclosure changes

FiledProof is deliberately conservative. It preserves source provenance, coverage boundaries, uncertainty, and abstains when a result cannot be established safely.

## Free and paid operations

Installing this plugin does not make a purchase or authorize payment.

FiledProof includes free research and discovery tools. Some specialist operations may require an explicit machine-payment authorization before execution. Payment authorizes execution only and does not change evidence confidence, verdict strength, research semantics, or source requirements.

## Important boundaries

FiledProof reports what companies filed with the U.S. Securities and Exchange Commission. It does not independently establish real-world truth, investment merit, legal materiality, accounting correctness, or economic significance.

## Publisher

Davisville Labs

Website: https://filedproof.com

Source package: https://github.com/davisvillelabs/filedproof-cursor-plugin

## License

The Cursor plugin wrapper in this repository is licensed under the MIT License. FiledProof's hosted service, research engine, data processing, payment systems, and private source code are not distributed by this repository and are not covered by that license.
