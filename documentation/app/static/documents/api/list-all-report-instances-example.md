#### Example Request

    GET https://lcp.points.com/v1/apps/<app-id>/reports/<report-id>/instances/
    Authorization: MAC id="...", ts="...", nonce="...", ext="...", mac="..."

#### Example Response

    200 OK
    {
      "instances": [
        {
          "contentType": "application/json",
          "createdAt": "2014-02-25T16:30:00Z",
          "status": "success",
          "links": {
            "self": {
              "href": "https://lcp.points.com/v1/apps/<app-id>/reports/<report-id>/instances/<id>"
            },
            "data": {
              "href": "https://lcp.points.com/v1/apps/<app-id>/reports/<report-id>/instances/<id>/data"
            },
            "report": {
              "href": "https://lcp.points.com/v1/apps/<app-id>/reports/<report-id>"
            }
          }
        },
        ...
      ]
    }









