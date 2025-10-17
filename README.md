# ALX GraphQL 0x00 - Character Queries

This project contains GraphQL query examples and their corresponding output files for character data retrieval.

## Project Structure

```
alx-graphql-0x00/
├── README.md
└── character/
    ├── README.md                    # Character-specific documentation
    ├── character-id-1.graphql       # Rick Sanchez query
    ├── character-id-1-output.json   # Rick Sanchez response
    ├── character-id-2.graphql       # Morty Smith query
    ├── character-id-2-output.json   # Morty Smith response
    ├── character-id-3.graphql       # Summer Smith query
    ├── character-id-3-output.json   # Summer Smith response
    ├── character-id-4.graphql       # Beth Smith query
    └── character-id-4-output.json   # Beth Smith response
```

## Overview

This project demonstrates GraphQL query structures and responses for character data. Each character query retrieves basic information including:

- Character ID
- Name
- Status (Alive/Dead/Unknown)
- Species
- Type/Subspecies
- Gender

## Getting Started

1. Navigate to the `character/` directory to explore individual GraphQL queries
2. Each `.graphql` file contains a query for a specific character
3. Corresponding `-output.json` files show the expected response format

## Characters Included

- **Rick Sanchez** (ID: 1) - Human Male, Alive
- **Morty Smith** (ID: 2) - Human Male, Alive
- **Summer Smith** (ID: 3) - Human Female, Alive
- **Beth Smith** (ID: 4) - Human Female, Alive

## Usage

These files serve as examples for:

- GraphQL query syntax and structure
- Expected JSON response formats
- Character data schema understanding

For detailed information about the character queries, see the [character directory README](./character/README.md).
