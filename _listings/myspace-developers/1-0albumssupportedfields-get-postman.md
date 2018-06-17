{
  "info": {
    "name": "My Space Get Albums Supported Fields",
    "_postman_id": "7f02999a-adad-4980-b40d-7a7e773c1a3f",
    "description": "Retrieves all supported fields.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Albums",
      "item": [
        {
          "id": "2dc9e5dc-dcdc-41a3-80e0-49a8fcc02caa",
          "name": "1.0.albums.personId._self.albumId.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.myspace.com",
              "path": [
                "1.0/albums/:personId/@self/:albumId"
              ],
              "variable": [
                {
                  "id": "albumId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "personId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves an album."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62c9399c-a2ce-4e8b-b279-ada69fa7d108"
            }
          ]
        },
        {
          "id": "54b42cd2-304f-4e66-b510-39f49e27248c",
          "name": "1.0.albums.personId._self.albumId.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.myspace.com",
              "path": [
                "1.0/albums/:personId/@self/:albumId"
              ],
              "variable": [
                {
                  "id": "albumId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "personId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Specifies Content Type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update an Album."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b38db909-5e35-4f56-991b-56fa47bcc146"
            }
          ]
        },
        {
          "id": "55eb6392-10a6-4620-8e7f-ccb68d0d6c01",
          "name": "1.0.albums.personId._self.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.myspace.com",
              "path": [
                "1.0/albums/:personId/@self"
              ],
              "query": [
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "msPrivacyLevel",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startIndex",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "personId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current user's albums."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38cd51f1-9767-4d9b-b216-12bc7d02756d"
            }
          ]
        },
        {
          "id": "75aaf4cb-166a-4002-aded-512bbcbd8786",
          "name": "1.0.albums.personId._self.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.myspace.com",
              "path": [
                "1.0/albums/:personId/@self"
              ],
              "variable": [
                {
                  "id": "personId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Specifies Content Type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Adding an Album."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d269da95-c04e-4392-984e-2ff93958fd8d"
            }
          ]
        },
        {
          "id": "be7acf7e-ed87-4c22-8445-2076c2c0d2de",
          "name": "1.0.albums._supportedFields.get",
          "request": {
            "url": "http://api.myspace.com/1.0/albums/@supportedFields?count=%7B%7D&fields=%7B%7D&format=%7B%7D&msPrivacyLevel=%7B%7D&startIndex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all supported fields."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca2b1c23-9c97-41dc-8a97-50a0e4639b0f"
            }
          ]
        }
      ]
    }
  ]
}