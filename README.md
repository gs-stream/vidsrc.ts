# vidsrc.ts
A cool vidsrc(.me/.net/.xyz/.in/.io) extractor in typescript.(proof of concept)

### FEATURES
- Nodejs & deno compatible (Deno : `deno run --allow-net vidsrc.ts`)
- Function (`tmdbScrape`) importable in any server libs (axios/hono/cf-workers)
- Deployable everywhere.

### USAGE (INPUT)
```ts
await tmdbScrape("TMDB_ID", "movie"); // movies (TMDB_ID:string,"movie")
await tmdbScrape("TMDB_ID","tv",1,1); // series (TMDB_ID:string,"tv",season:number,episode:number)
```

### RETURN TYPE

** supposed to change later.

```js
[
  {
    name: "",
    image: "",
    mediaId: "996",
    stream: "https://playlist.m3u8",
  }
]
```