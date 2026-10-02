# Database Schema

## Collection: contacts

| Field | Type | Required | Description |
|---|---|---|---|
| `_id` | ObjectId | Yes | MongoDB document identifier |
| `name` | String | Yes | Visitor name |
| `email` | String | Yes | Visitor email |
| `message` | String | Yes | Contact message |
| `createdAt` | Date | Automatic | Creation timestamp |
| `updatedAt` | Date | Automatic | Last update timestamp |

Mongoose creates the `contacts` collection from `server/models/Contact.js`.
