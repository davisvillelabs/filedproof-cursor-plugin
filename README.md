# FiledProof for Cursor

FiledProof is a read-only, primary-source SEC filing intelligence service for AI agents.

This Cursor plugin provides a no-cost FiledProof research surface for filing-grounded work without requiring the agent to independently retrieve, parse, align, and re-compare SEC filings.

## MCP server

`https://filedproof.davisvillelabs.com/mcp/marketplace`

The plugin connects Cursor directly to FiledProof's public Streamable HTTP marketplace endpoint. No API key, payment credential, or secret is stored in this repository.

## Free capabilities

The Cursor marketplace surface exposes standalone FiledProof operations that are designated free and zero-price in FiledProof's canonical product registry, including capabilities such as:

- resolving public-company issuers
- listing recent and bounded historical SEC filings
- searching filing evidence with exact provenance
- building answer-ready evidence packs
- building disclosure timelines
- verifying claims against SEC filings
- comparing two filings from the same issuer
- building reusable historical disclosure lineage
- building cross-company disclosure matrices

FiledProof is deliberately conservative. It preserves source provenance, coverage boundaries, uncertainty, and abstains when a result cannot be established safely.

## Marketplace boundary

This Cursor plugin exposes only standalone no-cost FiledProof research operations. Paid, internal, and paid-flow preflight operations are not listed by this endpoint and cannot be invoked through this plugin.

The free catalog is derived from FiledProof's canonical product registry with strict marketplace exclusions. A new standalone MCP operation explicitly classified as free with a zero price becomes eligible automatically when it follows FiledProof's canonical tool naming convention. Paid, internal, unregistered, unknown, and paid-flow preflight operations fail closed.

Installing or using this plugin does not make a purchase or authorize a payment.

## Important boundaries

FiledProof reports what companies filed with the U.S. Securities and Exchange Commission. It does not independently establish real-world truth, investment merit, legal materiality, accounting correctness, or economic significance.

## Publisher

Davisville Labs

Website: https://filedproof.davisvillelabs.com

Source package: https://github.com/davisvillelabs/filedproof-cursor-plugin

## License

The Cursor plugin wrapper in this repository is licensed under the MIT License. FiledProof's hosted service, research engine, data processing, payment systems, and private source code are not distributed by this repository and are not covered by that license.
