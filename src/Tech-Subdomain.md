# Subdomain

Like in the DNS, in the CNS hierarchy, a subdomain is a domain that is a part of another (main) domain. For example, if a domain offered an alternative alias address for receiving donation as part of their main CNS `pawket.xch`, it might use the subdomain `donate.pawket.xch`.

The CNS has a tree structure or hierarchy, which includes nodes on the tree being a domain name. A subdomain is a domain that is part of a larger domain. Each label may contain from `1` to `63` octets. The full domain name may not exceed a total length of `253` ASCII characters in its textual representation.

Different than traditional DNS, there are two ways to implement subdomains:

- **NFT Approach**. Subdomains can be NFT as main domain does, and they will be valid if: The issuer address is the address bound to main domain. Also, this means the subdomain would be invalidated when main domain's bound address changed.
- **Non-NFT Approach**. Subdomains work as resolver respond resolving result, and they will be valid if: The main domain bound a resolver address(A record or CNAME) to it, and the resolver resolves the corresponding subdomain.

## NFT Approach (Onchain Resolver)

CNS main domain owner only have issuer right over all these subdomains. Owner of main domain may:

- Invalidated all subdomains (NFT) at once by change the bound address of main domain.

Owner of main domain without ownership of subdomain cannot:

- Change ownership of the subdomain
- Change any bound property including address of this subdomain

In this approach, a delegated resolver is acceptable, any on-chain resolver service could serve subdomain with/without fees.

With this approach, main domain owner can issue the subdomain NFT with full customization ability, so the main domain owner can issue subdomain NFT with their own branding on the NFT image, or they can replace the traditional NFT with CNS NFT without losing any existing attribute, but with CNS merit.

## Non-NFT Approach (Offchain Resolver)

CNS domain owner have full ownership of all these subdomains. Owner of main domain may:

- Invalidated all subdomains (NFT) at once by change the bound address of main domain.
- Change ownership of the subdomain
- Change any bound property including address of this subdomain

In this approach, a dedicated resolver is required, some service provider may deliver a aggregated resolver service, but without onchain information, the resolver response cannot be validated by wallet client.

## Comparison

| Approach | Pros | Cons|
| --- | --- | ---|
| NFT Approach | ✅Onchain verification<br>✅Reuse or delegate onchain resolver<br>✅Customize NFT | ❌Cannot change ownership of subdomain<br>❌Cannot change bound property |
| Non-NFT Approach | ✅Full ownership of subdomain | ❌No onchain verification<br>❌Dedicated offchain resolver needed |