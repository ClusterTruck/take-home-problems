# ClusterTruck Take Home Problem

The following is a test designed to ensure you have a fundamental understanding of building data-­driven applications. It is not meant to be challenging, just to qualify your skills and open a conversation.

Please write the code in whatever environment you are comfortable. Also make the endpoint available publicly through whatever means you might have available and send the URL, login if necessary, and link to the code repository.

## Application Requirements

Your task is to build an HTTP endpoint that will receive a street address and return the drive time to the closest ClusterTruck kitchen utilizing the ClusterTruck Kitchen API and the [Google Maps Directions API](https://developers.google.com/maps/documentation/directions/).

### Example Request

```http
POST <YOUR URL>
Content-Type: application/json

{"address":"123 Main St, Anywhere, OH"}
```

OR

```sh
curl -X "POST" "http://www.example.com/url" \
     -H "Content-Type: application/json" \
     -d $'{"address": "123 Main St, Anywhere, OH"}'
```

### ClusterTruck Kitchens API

The following describes the kitchen API endpoint that will get you the `location` for each kitchen.

`curl -sH"Accept: application/vnd.api.clustertruck.com; version=2" https://api.staging.clustertruck.com/api/kitchens | \
python -m json.tool | less`
