{
  "info": {
    "name": "News Cred Author",
    "_postman_id": "132cf5f6-14f2-4d26-b880-247e92e05dc4",
    "description": "Returns an author that has written content available via this API.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "News",
      "item": [
        {
          "id": "1e404135-fec0-413f-b2b2-782ae28a0aef",
          "name": "getTopicGu]Articles",
          "request": {
            "url": "http://api.newscred.com/topic/{guid]/articles/?access_key=%7B%7D&article_filter_mode=%7B%7D&article_filter_name=%7B%7D&categories=%7B%7D&from_date=%7B%7D&get_topics=%7B%7D&guid=%7B%7D&has_images=%7B%7D&languages=%7B%7D&licensed=%7B%7D&media_types=%7B%7D&offset=%7B%7D&pagesize=%7B%7D&sort=%7B%7D&sources=%7B%7D&source_countries=%7B%7D&source_filter_mode=%7B%7D&source_filter_name=%7B%7D&to_date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of articles related to the specified topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ed133fc-6811-4b71-a36f-3e26447f081b"
            }
          ]
        },
        {
          "id": "fe330771-b1e7-474f-82ef-b4b458187feb",
          "name": "getArticles",
          "request": {
            "url": "http://api.newscred.com/articles/?access_key=%7B%7D&article_filter_mode=%7B%7D&article_filter_name=%7B%7D&boolean_operator=%7B%7D&categories=%7B%7D&exact=%7B%7D&from_date=%7B%7D&get_topics=%7B%7D&has_images=%7B%7D&languages=%7B%7D&licensed=%7B%7D&links=%7B%7D&max_length=%7B%7D&media_types=%7B%7D&min_length=%7B%7D&mm=%7B%7D&modified_since=%7B%7D&offset=%7B%7D&query=%7B%7D&query_fields=%7B%7D&safe_search=%7B%7D&sort=%7B%7D&sources=%7B%7D&source_countries=%7B%7D&source_filter_mode=%7B%7D&source_filter_name=%7B%7D&topics=%7B%7D&topic_filter_mode=%7B%7D&topic_filter_name=%7B%7D&to_date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of articles according to the specified set of parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a6163b2-6676-46ec-b5f7-7fbb53fd998f"
            }
          ]
        }
      ]
    },
    {
      "name": "Author",
      "item": [
        {
          "id": "8ca5561b-a05f-402e-b157-f863512404f5",
          "name": "getAuthor",
          "request": {
            "url": "http://api.newscred.com/author/?access_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an author that has written content available via this API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c5afb43-f5cc-47e0-8041-f1d49282791e"
            }
          ]
        }
      ]
    }
  ]
}