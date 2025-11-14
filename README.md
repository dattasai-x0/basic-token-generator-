# Basic Token Creator Smart Contract

## Project Title
**Basic Token Creator** - A Soroban-based smart contract for creating and managing custom tokens on the Stellar network.

## Project Description
The Basic Token Creator is a lightweight smart contract built with Soroban SDK that enables users to create, configure, and manage custom tokens (assets) on the Stellar blockchain. This contract provides a simple interface for defining token parameters such as name, symbol, total supply, and decimals, while maintaining comprehensive tracking and statistics of all created tokens on the platform.

## Project Vision
To democratize token creation on the Stellar network by providing an accessible, user-friendly smart contract that allows developers and businesses to create custom tokens without complex configuration or deep blockchain expertise. This contract serves as a foundation for decentralized applications, community tokens, and custom asset creation on Stellar.

## Key Features

**Token Creation**
- Users can create new custom tokens by specifying essential parameters like name, symbol, total supply, and decimal places
- Each token receives a unique identifier and timestamp of creation
- Creator information is recorded for accountability and tracking

**Token Management**
- Retrieve detailed information about any created token using its unique token ID
- Deactivate tokens when they are no longer needed, while maintaining historical records
- All token data is stored immutably on the Stellar blockchain

**Statistics Tracking**
- Real-time tracking of total tokens created on the platform
- Monitor active and inactive token counts
- Access comprehensive statistics for platform analytics and reporting

**Security and Data Persistence**
- Automatic TTL (Time-To-Live) extension ensuring data persistence
- Ledger timestamp integration for accurate creation and modification timestamps
- Default value handling for missing token data

## Contract Functions

### `create_token(name, symbol, total_supply, decimals, creator_address) → u64`
Creates a new custom token with specified parameters and returns its unique token ID.

### `get_token_details(token_id) → TokenMetadata`
Retrieves complete metadata and configuration details of a specific token by its ID.

### `deactivate_token(token_id) → void`
Deactivates an active token and updates platform statistics accordingly.

### `get_token_stats() → TokenStats`
Returns current platform-wide token creation statistics including total, active, and inactive token counts.

## Future Scope

**Enhanced Token Features**
- Support for token burning mechanisms to reduce total supply
- Minting capabilities for token creators to increase supply
- Token transfer and trading functionality with fee structures

**Access Control**
- Role-based authorization (admin, creator, user roles)
- Creator-only token modification privileges
- Multi-signature approval for critical operations

**Advanced Statistics**
- Detailed token creation timeline and historical data
- Token holder statistics and distribution tracking
- Platform growth metrics and analytics dashboards

**Integration Capabilities**
- API endpoints for frontend integration
- Cross-contract communication for DeFi protocols
- Integration with token swaps and liquidity pools

**Governance Features**
- Decentralized governance tokens backed by this contract
- Token voting mechanisms for platform decisions
- Community-driven token validation and approval processes

---

**Built with:** Soroban SDK (Rust)  
**Network:** Stellar Blockchain  
**License:** Open Source