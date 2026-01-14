# Architecture Overview – Minimal Service Example

## System Goals
- Simplicity over flexibility
- Low operational overhead
- Easy to understand and modify

## Non-Goals
- High availability across regions
- Real-time processing
- Complex scaling strategies

## High-Level View

Client
  |
  v
HTTP API
  |
  v
Relational Database

## Major Components

### HTTP API
- Accepts incoming requests
- Validates input
- Persists data
- Returns synchronous responses

Responsibilities:
- Input validation
- Error handling
- Basic authentication (if required)

### Database
- Stores submitted records
- Acts as the system of record

Responsibilities:
- Data durability
- Simple query support

## External Dependencies
- Database (e.g. PostgreSQL)
- No third-party APIs required

## Data Flow
1. Client sends request to API
2. API validates input
3. API writes record to database
4. API returns success or error

## Scaling Assumptions
- Low to moderate request volume
- Vertical scaling is sufficient initially
- Database is the primary bottleneck

## Constraints
- Small team
- Limited operational capacity
- Preference for managed services
