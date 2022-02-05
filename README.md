# Pinboard API Proxy

For whatever reason the [Pinboard API](https://pinboard.in/howto/#api) doesn't have CORS enabled — so you can't make API calls directly from the browser.
This tiny Vercel serverless function acts as a proxy to the Pinboard API allowing requests from all origins.

## Setup

1. Fork this repo
2. Link it to your Vercel dashboard
3. That's it 👍

## Usage

Call `/api/*` just like if it was the Pinboard API.

For example, `/api/v1/posts/all?format=json` will be proxied to `https://api.pinboard.in/v1/posts/all?format=json`.
