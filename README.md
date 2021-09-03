# url-shortener

This is a url shortner service that takes a long url from the user and make it short.

## How to use

- Clone the repository using `git clone https://github.com/ranopriyo-neogy/url-shortener.git`
- Get into the project folder using `cd url_shortner_service`
- Run `docker-compose up`
- From any REST Client hit - ``http://localhost:5000/api/url/shorten` with `POST` operation.
- Pass a long url in below format:
```
{
    "longUrl": ""
}
```
- The Response will be having the short url.