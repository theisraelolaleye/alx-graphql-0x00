# Episode and Character Pagination - GraphQL Queries

## Overview
This directory contains GraphQL queries for both episode data retrieval and character pagination from the Rick and Morty API.

## Endpoint
https://rickandmortyapi.com/graphql

## File Structure

### Episode Queries
- `episode-page-1.graphql` - Episode query for page 1
- `episode-page-2.graphql` - Episode query for page 2
- `episode-page-3.graphql` - Episode query for page 3
- `episode-page-4.graphql` - Episode query for page 4

### Character Pagination Queries
- `characters-page-2.graphql` - Characters pagination query for page 2
- `characters-page-2-output.json` - API response for page 2
- `characters-page-3.graphql` - Characters pagination query for page 3
- `characters-page-3-output.json` - API response for page 3
- `characters-page-4.graphql` - Characters pagination query for page 4
- `characters-page-4-output.json` - API response for page 4

## Query Types

### Episode Queries
Retrieve specific episode information using episode IDs or pagination.

**Example Episode Query:**
```graphql
query {
  episode(id: 1) {
    id
    name
    air_date
    episode
  }
}
```

### Character Pagination Queries
Retrieve paginated character data with pagination info.

**Example Character Pagination Query:**
```graphql
query {
  characters(page: 2) {
    info {
      count
      pages
      next
      prev
    }
    results {
      id
      name
      status
      species
      type
      gender
      image
    }
  }
}
```

## Usage
1. Use episode queries to retrieve specific episode data by ID
2. Use character pagination queries to navigate through character pages
3. Each query demonstrates different aspects of the Rick and Morty GraphQL API
4. Output files show expected response structure for character pagination queries

## API Schema Fields

### Episode Fields
- `id` - Episode identifier
- `name` - Episode title
- `air_date` - Original air date
- `episode` - Episode code (e.g., "S01E01")

### Character Fields
- `id` - Character identifier
- `name` - Character name
- `status` - Character status (Alive, Dead, Unknown)
- `species` - Character species
- `type` - Character type/subspecies
- `gender` - Character gender
- `image` - Character image URL

### Pagination Info
- `count` - Total number of items
- `pages` - Total number of pages
- `next` - Next page number (null if last page)
- `prev` - Previous page number (null if first page)