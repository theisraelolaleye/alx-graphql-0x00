# Character GraphQL Queries

This directory contains GraphQL queries and their corresponding output files for character data retrieval.

## Files Structure

Each character has two associated files:

- `character-id-{n}.graphql` - The GraphQL query file
- `character-id-{n}-output.json` - The JSON response/output file

## Available Characters

| ID  | Name         | Status | Species | Gender |
| --- | ------------ | ------ | ------- | ------ |
| 1   | Rick Sanchez | Alive  | Human   | Male   |
| 2   | Morty Smith  | Alive  | Human   | Male   |
| 3   | Summer Smith | Alive  | Human   | Female |
| 4   | Beth Smith   | Alive  | Human   | Female |

## GraphQL Query Structure

All character queries follow the same structure, requesting the following fields:

- `id` - Character identifier
- `name` - Character's full name
- `status` - Current status (Alive, Dead, Unknown)
- `species` - Character's species
- `type` - Character type/subspecies
- `gender` - Character's gender

## Usage

You can use these GraphQL queries as examples or templates for querying character data from a GraphQL API endpoint that supports this schema structure.

### Example Query

```graphql
query {
	character(id: 1) {
		id
		name
		status
		species
		type
		gender
	}
}
```

### Example Response

```json
{
	"data": {
		"character": {
			"id": "1",
			"name": "Rick Sanchez",
			"status": "Alive",
			"species": "Human",
			"type": "",
			"gender": "Male"
		}
	}
}
```
