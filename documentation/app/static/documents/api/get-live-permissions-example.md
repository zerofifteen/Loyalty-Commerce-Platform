#### Example Request

    GET https://lcp.points.com/v1/apps/<app-id>/live-permissions/<id>
    Authorization: MAC id="...", ts="...", nonce="...", ext="...", mac="..."

#### Example Response

    200 OK
    {
      "links": {
        "self": {
          "href": "https://lcp.points.com/v1/apps/<app-id>/live-permissions/<id>"
        }
      },
      "loyaltyProgram": "https://lcp.points.com/v1/lps/<lp-id>",
      "operations": ["mvs", "debits", "credits"]
    }


