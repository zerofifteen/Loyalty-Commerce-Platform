#### Example Request

    GET https://lcp.points.com/v1/accounts/
    Authorization: MAC id="...", ts="...", nonce="...", ext="...", mac="..."

#### Example Response

    200 OK
    {
      "accountCredentials": [
        {
          "links": {
            "self": {
              "href": "https://lcp.points.com/v1/accounts/<id>/account-credentials/<ac-id>"
            }
          },
          "macAlgorithm":"HMAC-SHA1",
          "macKey":"<macKey>",
          "macKeyIdentifier":"<macKeyIdentifier>"
        }
      ],
      "email": "<email>",
      "firstName": "<firstName>",
      "lastName": "<lastName>",
      "links": {
          "self": {
            "href": "https://lcp.points.com/v1/accounts/<id>"
          },
          "friendly": {
            "href": "https://lcp.points.com/v1/accounts/<email>"
          }
      },
      "organizationName": "<organizationName>",
      "phone": "<phone>"
    }

