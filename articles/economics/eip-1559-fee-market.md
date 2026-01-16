# EIP-1559: Fee Market Change

## Metadata

- **Title**: EIP-1559: Fee Market Change for ETH 1.0 Chain
- **Description**: Understanding Ethereum's transaction fee mechanism that introduced base fees and burned ETH, fundamentally changing the economics of the network.
- **Link**: https://eips.ethereum.org/EIPS/eip-1559
- **Date Added**: 2024-01-16
- **Date Published**: 2021-08-05
- **Tags**: `eip`, `gas`, `economics`, `protocol-upgrade`, `eip-1559`

---

## Summary

EIP-1559 fundamentally reformed Ethereum's transaction fee mechanism by introducing a base fee that is burned and an optional priority fee (tip) that goes to miners/validators. This proposal went live in the London hard fork in August 2021.

Prior to EIP-1559, users submitted bids for block space in a first-price auction, leading to inefficient pricing and poor user experience. The new mechanism uses an algorithmic base fee that adjusts based on network congestion, making fees more predictable.

The burning of base fees has significant economic implications, potentially making ETH deflationary during periods of high network usage. This creates a direct link between network usage and ETH's monetary policy, aligning the interests of ETH holders with network activity.

EIP-1559 improved transaction fee predictability, reduced overpayment, and created a more efficient fee market. Combined with Proof-of-Stake post-Merge, the burning mechanism has indeed made ETH deflationary at times.

## Key Concepts

- **Base Fee**: A dynamically adjusting fee that all transactions must pay, which is burned (removed from circulation). It increases when blocks are full and decreases when they're under-utilized.

- **Priority Fee (Tip)**: An optional additional fee paid directly to validators to incentivize inclusion. Users can set this to speed up transaction processing during congestion.

- **Fee Burning**: The base fee is permanently removed from ETH's supply. This creates deflationary pressure when network usage is high, offsetting or exceeding the issuance from staking rewards.

- **Block Size Flexibility**: Blocks can vary between 0 and 2x the target gas limit (15M to 30M gas), allowing the network to absorb short-term demand spikes while maintaining average block sizes.

## Important Quotes or Highlights

> "The base fee is burned, creating a deflationary pressure on ETH supply that increases with network usage."

> "This proposal makes Ethereum's monetary policy more predictable and ties it directly to network utility."

## Personal Notes

EIP-1559 was one of the most anticipated upgrades because it addressed a major UX issue (unpredictable fees) while also introducing interesting economic dynamics. The fee burning mechanism essentially makes every user a "stakeholder" in ETH's economics.

Key observations:
- Wallets improved dramatically with better fee estimation
- The "ultrasound money" narrative emerged from the deflationary potential
- Combined with PoS, some blocks see more ETH burned than issued
- Gas wars still happen through priority fees, but the base fee provides a floor

Economic implications:
- ETH becomes more attractive to hold during high usage
- Validators' revenue shifted from fees to tips + issuance
- The mechanism creates better alignment between users and ETH holders

Questions to explore:
- What happens to fee dynamics during extreme congestion?
- How does this compare to other fee mechanisms (like Solana's)?
- Long-term implications of variable monetary policy tied to usage?

## Related Articles

- [Article about The Merge] (articles/consensus/the-merge-pos-transition.md)
- [Article about MEV] (to be added)
- [Article about Layer 2 scaling] (to be added)

## References

- https://eips.ethereum.org/EIPS/eip-1559
- https://ethereum.org/en/developers/docs/gas/
- https://notes.ethereum.org/@vbuterin/eip-1559-faq
- https://ultrasound.money/ (visualizing the burn)
