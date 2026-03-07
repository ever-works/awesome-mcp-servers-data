## Overview

Shopify provides official MCP servers as API endpoints that provide structured access to Shopify's commerce data, including products, cart operations, customer information, and store policies. The Storefront MCP server offers tools to help customers browse and buy from a specific store.

## Key Features

- **Product Discovery**: Natural-language search with recommendations
- **Cart Management**: Create carts, add/remove items, complete checkout
- **Store Information**: Answer questions about policies, shipping, returns, FAQs
- **Order Management**: Track order status and process returns
- **Interactive UI Components**: MCP UI for visual commerce experiences
- **GraphQL API Integration**: Access full Shopify GraphQL capabilities
- **Multi-Store Support**: Manage multiple Shopify stores

## Official MCP Servers

**1. Storefront MCP Server**
- Store catalog queries
- Cart operations
- General store information
- Customer-facing commerce operations

**2. Customer Accounts MCP Server**
- Order tracking
- Return management
- Account information access
- Customer self-service

**3. Dev MCP Server**
- Search Shopify docs
- Explore API schemas
- Build Shopify Functions
- Get API answers and examples

## Core Capabilities

**Product Catalog:**
- Search products by natural language
- Browse collections
- View product details
- Check inventory availability
- Product recommendations
- Filter by price, category, attributes

**Cart & Checkout:**
- Create shopping carts
- Add items to cart
- Update quantities
- Remove items
- Apply discount codes
- Calculate totals with tax/shipping
- Complete checkout process

**Order Operations:**
- Track order status
- View order history
- Process returns and exchanges
- Print invoices
- Manage shipping addresses

**Store Management:**
- Store policies (shipping, returns, privacy)
- FAQ access
- Contact information
- Operating hours
- Location details

## MCP UI Enhancement

MCP UI extends the Model Context Protocol to enable AI agents to return fully interactive UI components, solving the challenge that commerce experiences require visual and interactive elements:

- Product selectors
- Image galleries
- Cart flows
- Checkout forms
- Order summaries
- Interactive filters

## Use Cases

**Automated Order Fulfillment:**
- Order processing workflows
- Shipping status updates
- Inventory synchronization
- Multi-channel management

**Inventory Management:**
- Sync product data across platforms
- Real-time stock updates
- Price synchronization
- SKU management

**Customer Data:**
- Extract customer data for CRM
- Targeted marketing campaigns
- Customer segmentation
- Behavior analysis

**Analytics & Reporting:**
- Custom sales reports
- Product performance analysis
- Customer insights
- Revenue tracking

## GraphQL API Access

Community MCP servers enable interaction with Shopify store data through GraphQL API:

- Product management
- Customer management
- Order management
- Inventory control
- Collections and categories
- Metafields and custom data

## Natural Language Examples

"Show me all products in the electronics category"
"Add this product to cart"
"What's your return policy?"
"Track my order #12345"
"Find products similar to this one"
"Apply discount code SUMMER2026"
"What are the shipping options?"

## Store Information Access

- Shipping policies
- Return and exchange policies
- Privacy policy
- Terms of service
- Payment options
- Contact details
- Store hours
- Physical locations

## Product Search Features

- **Natural Language**: "Blue running shoes under $100"
- **Semantic Search**: Understanding intent beyond keywords
- **Filters**: Price, category, brand, size, color
- **Sorting**: Price, popularity, newest, rating
- **Recommendations**: Related products, frequently bought together

## Cart Management

**Cart Operations:**
- Create new cart
- Add line items
- Update quantities
- Remove items
- Clear cart
- Apply discounts
- Calculate totals

**Cart Persistence:**
- Save for later
- Share cart links
- Cart abandonment recovery
- Cross-device sync

## Checkout Process

- Shipping address collection
- Payment method selection
- Order review
- Order confirmation
- Receipt generation
- Email notifications

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- Cursor
- VS Code with Copilot
- ChatGPT (with MCP support)
- Custom MCP implementations

## Integration Patterns

**Customer Service Bot:**
1. Customer asks product question
2. AI searches catalog
3. Returns relevant products
4. Assists with cart and checkout

**Inventory Sync:**
1. Detect inventory changes
2. Update across platforms
3. Trigger restocking alerts
4. Sync pricing updates

## Security & Authentication

- OAuth 2.0 authentication
- Storefront API access tokens
- Admin API permissions
- Rate limiting
- Webhook verification
- PCI compliance for payments

## Rate Limits

- Storefront API: 2 requests per second per store
- Admin API: Varies by plan tier
- GraphQL: Cost-based limits
- Bulk operations: Special handling

## Customization

- Custom fields (metafields)
- Product variants
- Custom checkout experiences
- Branded storefronts
- Multi-language support
- Multi-currency support

## Analytics Integration

- Google Analytics
- Facebook Pixel
- Custom tracking
- Conversion tracking
- A/B testing support

## Multi-Channel Commerce

- Online store
- Point of Sale (POS)
- Social commerce (Facebook, Instagram)
- Marketplace integration
- Mobile apps

## Developer Tools

- Shopify CLI
- Theme development
- App development
- Webhook management
- API playground
- GraphQL explorer

## Performance Optimization

- CDN for product images
- Cached API responses
- Lazy loading
- Optimized queries
- Bulk operations

## Compliance

- GDPR compliance
- PCI DSS for payments
- Accessibility standards
- Data portability
- Right to deletion

## Pricing

Shopify pricing tiers:

- **Basic**: Starting tier with essential features
- **Shopify**: Mid-tier with advanced features
- **Advanced**: Enterprise features
- **Plus**: Enterprise-grade for high volume

MCP servers are free to use with Shopify subscription.