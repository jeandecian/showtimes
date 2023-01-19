# List all movies

**Endpoint** : `GET /api/v1/movies`

## Query Parameters

| Parameter                  | Type    | Required | Description          	 |
|----------------------------|---------|----------|--------------------------|
| `language`                 | string  | optional | Movie language           |
| `marketLanguageCodeFilter` | boolean | optional | Enable `language` filter |
| `movieType`                | number  | optional | Movie type               |
| `showTimeType`             | number  | optional |							 |
| `showtimeStatus`           | number  | optional |							 |
| `skip`                     | number  | optional |	Skip first `n` movie(s)  |
| `take`                     | number  | optional | Size of results          |

## Response

| Field                      | Type         | Description                                  |
|----------------------------|--------------|----------------------------------------------|
| `data`                     | object array | Array of Movie objects                       |
| `isWatchListed`            | boolean      |                                              |
| `id`                       | number       | Movie identifier                             |
| `presentationType`         | string       | Movie type                                   | 
| `name`                     | string       | Movie title                                  |
| `releaseDate`              | string       |                                              |
| `firstShowStartDate`       | string       |                                              |
| `marketLanguageCode`       | string       | Market language code                         |
| `isNowPlaying`             | boolean      | Movie is now playing                         |
| `isComingSoon`             | boolean      | Movie is coming soon                         |
| `isReleasingSoon`          | boolean      | Movie is releasing soon                      |                          
| `isEvent`                  | boolean      | Movie is an event                            |
| `hasShowtimes`             | boolean      | Movie showtimes available                    |
| `hasPosterImage`           | boolean      | Movie poster image available                 |
| `smallPosterImageUrl`      | string       | URL to the small poster image                |
| `mediumPosterImageUrl`     | string       | URL to the medium poster image               |
| `largePosterImageUrl`      | string       | URL to the large poster image                |
| `mobileBackgroundImageUrl` | string       | URL to the mobile background image           |
| `mpaaRating`               | object       | Motion Picture Association of America rating |
| `province`                 | string       | Province                                     |
| `ratingTitle`              | string       | Rating's title                               |
| `ratingDescription`        | string       | Rating's description                         |
| `warning`                  | string       | Rating's warning                             |
| `imageUrl`                 | string       | Rating's image                               |
| `formats`                  | string array | Movie format(s)                              |
| `brightcoveVideoId`        | number       | Brightcove video identifier                  |
| `urlSlug`                  | string       | URL Slug                                     |
| `duration`                 | string       | Movie duration                               |
| `vistaEventCode`           | string       |                                              |
| `vistaEventCodeVIP`        | string       |                                              |
| `seriesTicketingUrl`       | string       |                                              |
| `seriesTicketingVIPUrl`    | string       |                                              |
| `runtime`                  | number       | Runtime in minutes                           |
| `skip`                     | number       | Skip first `n` movie(s)                      |
| `take`                     | number       | Size of results                              |
| `totalCount`               | number       | Size of total results                        |
| `status`                   | number       |                                              |
| `message`                  | string       | Message                                      |
| `messageDetails`           | string       | Message details                              |
| `apiVersionNumber`         | string       | API version number                           |

```json
{
	"data": [
    	{
			"isWatchListed": false,
			"id": 00000,
			"presentationType": "",
			"name": "",
			"releaseDate": "2015-10-20T00:00:00",
			"firstShowStartDate": "2015-10-20T00:00:00",
			"marketLanguageCode": "",
			"isNowPlaying": true,
			"isComingSoon": false,
			"isReleasingSoon": false,
			"isEvent": false,
			"hasShowtimes": true,
			"hasPosterImage": true,
			"smallPosterImageUrl": "",
			"mediumPosterImageUrl": "",
			"largePosterImageUrl": "",
			"mobileBackgroundImageUrl": "",
			"mpaaRating": {
				"province": "",
				"ratingTitle": "",
				"ratingDescription": "",
				"warning": "",
				"imageUrl": ""
			},
			"formats": [],
			"brightcoveVideoId": 0,
			"urlSlug": "lorem-ipsum",
			"duration": "1h 09m",
			"vistaEventCode": "",
			"vistaEventCodeVIP": "",
			"seriesTicketingUrl": "",
			"seriesTicketingVIPUrl": "",
			"runtime": 69
		}
	],
	"skip": 0,
	"take": 69,
	"totalCount": 420,
	"status": 1,
	"message": "",
	"messageDetails": "",
	"apiVersionNumber": ""
}
```