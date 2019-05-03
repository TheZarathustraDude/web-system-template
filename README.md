# Be Current with Currents

## Description
- The system shows a few News articles found across the internet.

 The main entity of this WEB systems is a Quote.
- Entity has these attributes:
    - ID - String
    ```
       - Joi.string().max(50);
    ```
    - author - String, author of News article.
    ```
       - Joi.string().max(200);
    ```
    - source URL - String, which defines URL to the source of News article.
    ```
       - No Restrictions
    ```
    - published -  Date string, which defines when the News article was published by the Author.
    ```
       - Joi.string().max(200);
    ```
    - title - String, which defines the title of News article.
    ```
       -  Joi.string().max(200);
    ```
    - language - String, which defines language of the News article.
    ```
       - Joi.string().max(200);
    ```

## API definition
- The main information that this WEB system GET from API is Random Quote and Random Meme.
- API methods (used by this WEB system):
    - GET News articles:
        ```
        - GET https://api.currentsapi.services/v1/latest-news
        ```
        - 404 {"status":404,"message":"No route found"}
    - GET News articles that are english:
        ```
        - GET https://api.currentsapi.services/v1/search?language=en
        ```
        - 404 {"status":404,"message":"No route found"}
    - GET News articles that have a keyword:
        ```
        - GET https://api.currentsapi.services/v1/search?keyword=Trump
        ```
       - 404 {"status":404,"message":"No route found"}
    - POST News article url:
       ```
        - POST /api/url/:id/url
        ```
## UI definition
```
- https://wireframe.cc/thBVy4
```
