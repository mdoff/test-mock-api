# test-mock-api
Simple mock express.js api

## Endpoints

### Get all frameworks:
Url: `/api/frameworks`
Schema:
```ts
{
  "description": string
  "id": string,
  "imageUrl": string,
  "stars": number,
  "github": string,
  "active": boolean
}[]
```

### Get single framework:
Url: `/api/frameworks/:framework_name`
Schema:
```ts
{
  "description": string
  "id": string,
  "imageUrl": string,
  "stars": number,
  "github": string,
  "active": boolean,
  "languages": {
    "language": string,
    "id": string,
    "imageUrl": string,
    "frameworks": string[]
  }[]
}
```

### Get all languages:
Url: `/api/languages`
```ts
{
    "language": string,
    "id": string,
    "imageUrl": string,
    "frameworks": string[]
}[]
```

### Get single language:
Url: `/api/languages/:language_name`
```ts
{
    "language": string,
    "id": string,
    "imageUrl": string,
    "frameworks": string[]
}
```
