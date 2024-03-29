# GraphQL Project with Go

## Overview

This project is a Golang application that utilizes GraphQL to manage categories and courses. It provides a flexible and efficient way to query and retrieve information about categories, courses, and their relationships.

## Getting Started

Follow these steps to set up and run the project locally:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/RaphaelMarquesMartorella/graphql-go.git
   
   cd graphql-go
   
   go mod tidy
   
   go run cmd/server/server.go
   ```

## Features

### Access GraphQL Playground

Open your web browser and navigate to http://localhost:8080 to access the GraphQL Playground. This interactive environment allows you to test and execute the provided queries in real-time.

### Queries

Retrieve information about all available data from categories and courses.

```graphql
query queryCategories {
  categories {
    id
    name
    description
  }
}

query queryCourses {
  courses {
    id
    name
    description
  }
}

query queryCategoriesWithCourses {
  categories {
    id
    name
    courses {
      id
      name 
    }
  }
}

query queryCoursesWithCategory {
  courses {
    id
    name
    description
    category {
      id
      name
      description
    }
  }
}

```
