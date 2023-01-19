# Endpoints

## Movies

| Endpoint                                         | Query Parameters | Description                          |
|--------------------------------------------------|------------------|--------------------------------------|
| `GET /api/v1/movies`                             | Optional         | Movies                               |
| `GET /api/v1/movies/:id`                         |                  | Movie information                    |
| `GET /api/v1/movies/:id/availabletheatres`       |                  | Available theatres for movie         |
| `GET /api/v1/movies/:id/availabletheatres/dates` | Optional         | Available dates by theatre for movie |

## Showtimes

| Endpoint                                   | Query Parameters | Description |
|--------------------------------------------|------------------|-------------|
| `GET /api/v1/showtimes`                    | Required         | Showtimes   |

## Theatres

| Endpoint                                   | Query Parameters | Description |
|--------------------------------------------|------------------|-------------|
| `GET /api/v1/theatres`                     | Optional         | Theatres    |