# Project Name

## Overview

This project is a Golang application that utilizes GraphQL to manage categories and courses. It provides a flexible and efficient way to query and retrieve information about categories, courses, and their relationships.

## Features

### Query Categories

Retrieve information about all available categories.

```graphql
query queryCategories {
  categories {
    id
    name
    description
  }
}
```

```
query queryCourses {
  courses {
    id
    name
    description
  }
}
```
