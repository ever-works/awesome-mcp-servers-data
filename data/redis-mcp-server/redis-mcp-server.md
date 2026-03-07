## Overview

The official Redis MCP Server is a natural language interface designed for agentic applications to efficiently manage and search data in Redis. It integrates seamlessly with MCP clients, enabling AI-driven workflows to interact with structured and unstructured data in Redis.

## Key Features

- **Natural Language Queries**: AI agents can query and update Redis using natural language
- **Full Redis Support**: Complete support for hashes, lists, sets, sorted sets, streams, and more
- **Search & Filtering**: Efficient data retrieval with advanced filtering
- **Scalable & Lightweight**: High-performance data operations
- **Key-Value Operations**: Set, get, delete, and list operations
- **Optional Expiration**: Time-to-live (TTL) support for keys
- **Pub/Sub**: Publish-subscribe messaging capabilities
- **Atomic Operations**: Increment, decrement, and other atomic operations

## Supported Data Structures

**Strings:**
- Simple key-value pairs
- Binary-safe storage
- String manipulation
- Numerical operations

**Hashes:**
- Field-value pairs within keys
- Efficient for object storage
- Partial updates
- Field-level operations

**Lists:**
- Ordered collections
- Push/pop operations
- Range retrieval
- Blocking operations

**Sets:**
- Unordered unique elements
- Set operations (union, intersection, difference)
- Member testing
- Random element selection

**Sorted Sets:**
- Scored members
- Range queries by score or rank
- Leaderboard implementations
- Priority queues

**Streams:**
- Append-only log structure
- Consumer groups
- Message acknowledgment
- Real-time data feeds

## Available Operations

**Basic Operations:**
- GET: Retrieve value by key
- SET: Store key-value pair
- DELETE: Remove key
- EXISTS: Check key existence
- KEYS: List keys matching pattern
- EXPIRE: Set key expiration

**List Operations:**
- LPUSH/RPUSH: Add to list
- LPOP/RPOP: Remove from list
- LRANGE: Get list range
- LLEN: Get list length

**Hash Operations:**
- HGET/HSET: Get/set hash field
- HGETALL: Get all hash fields
- HDEL: Delete hash field
- HKEYS: List hash field names

**Set Operations:**
- SADD: Add set member
- SMEMBERS: List set members
- SISMEMBER: Check membership
- SUNION/SINTER: Set operations

**Pub/Sub:**
- PUBLISH: Send message to channel
- SUBSCRIBE: Listen to channel
- UNSUBSCRIBE: Stop listening

## Use Cases

**Session Management:**
- Store and retrieve user session data
- Implement session timeouts with TTL
- Fast session validation
- Distributed session storage

**Caching:**
- Cache frequently accessed data
- Reduce database load
- Improve application performance
- Implement cache invalidation strategies

**Real-Time Data:**
- Manage real-time data feeds
- Implement message queues
- Track live metrics
- Process stream data

**Rate Limiting:**
- Track API usage
- Implement sliding window rate limits
- Prevent abuse
- Throttle requests

**Leaderboards:**
- Real-time score tracking
- Ranked listings
- Gaming applications
- Competition management

## Integration

The Model Context Protocol (MCP) is a standard that lets AI agents access data and perform actions. Using MCP, your server can publish a set of commands that are usable by any MCP-compatible client app (such as Claude Desktop or VS Code).

## Available Implementations

**1. redis/mcp-redis** (Official)
- Official Redis implementation
- Complete feature set
- Production-ready
- Actively maintained

**2. GongRzhe/REDIS-MCP-Server**
- Community implementation
- Pushed to official servers repository
- Standardized tools for LLM interaction

**3. prajwalnayak7/mcp-server-redis**
- Supports Redis Server and AWS MemoryDB
- Specialized for caching use cases
- In-memory and key-value storage focus

**4. Azure Redis Tools** (Microsoft)
- Azure Cache for Redis integration
- Cloud-specific features
- Azure ecosystem integration

## Natural Language Examples

"Store user session for ID 12345"
"Get the value of cache:user:profile:123"
"Set a 5-minute expiration on session:abc"
"Add item to shopping cart list"
"Publish notification to alerts channel"
"Increment page view counter"

## Configuration

Typical configuration:

- **Host**: Redis server hostname
- **Port**: Redis port (default 6379)
- **Password**: Optional authentication
- **Database**: Database number (0-15)
- **TLS**: Optional encrypted connection
- **Connection Pool**: Connection pooling settings

## Performance Characteristics

- **Latency**: Sub-millisecond operations
- **Throughput**: 100k+ operations per second
- **Memory**: In-memory for ultra-fast access
- **Persistence**: Optional disk persistence
- **Replication**: Master-replica support
- **Clustering**: Horizontal scaling

## High Availability

**Redis Sentinel:**
- Automatic failover
- Monitoring and notifications
- Configuration management

**Redis Cluster:**
- Sharding across multiple nodes
- Automatic data partitioning
- High availability
- Horizontal scalability

## Compatible MCP Clients

- Claude Desktop
- Claude Code
- VS Code with Copilot
- Cursor
- Continue
- Custom MCP implementations

## Security Features

- Password authentication
- ACL (Access Control Lists)
- TLS/SSL encryption
- Command renaming
- Protected mode
- IP filtering

## Data Persistence

**RDB (Redis Database):**
- Point-in-time snapshots
- Compact storage
- Fast restarts

**AOF (Append Only File):**
- Log every write operation
- Better durability
- Reconstructible on restart

**Hybrid:**
- Combine RDB and AOF
- Best of both approaches

## Cloud Deployments

- **Redis Cloud**: Fully managed Redis
- **AWS ElastiCache**: Redis on AWS
- **Azure Cache for Redis**: Microsoft Azure
- **Google Cloud Memorystore**: Google Cloud Platform

## Monitoring

- INFO command for server statistics
- MONITOR for real-time command tracing
- SLOWLOG for slow queries
- CLIENT LIST for connection info
- Memory usage tracking

## Pricing

Free and open-source MCP server. Redis deployment costs depend on:

- Self-hosted: Infrastructure costs only
- Redis Cloud: Based on memory and throughput
- Cloud providers: Per instance pricing