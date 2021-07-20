# Epidemic Sound Mobile Browser

The goal of this project is to assess your mobile development skills, while we prefer you have your own code to walk through with us, this coding test exists. 

- **Project Name:** Catalog Browser
- **Project Goal:** Create a project that queries our app gateway and lays out items
- **Technology:** Any mobile technology is fine, but please keep in mind we are developing our apps in Swift and Kotlin 😇
- **Deliverables:** Solution should be sent to your talent partner for evaluation. 

**Description:** Build a mobile client that consumes part of our API. Firstly, laying out the catalog, with images 🌉, then browsing to the tracks in the in a given mood/genre and showing some of the track metadata.

**API to Consume:** `agw.epidemicsound.com` is our RESTful JSON API, and has some endpoints that are open to the public.

`https://agw.epidemicsound.com/catalog` returns a list of genres and moods along with image urls for you to use. 

`https://agw.epidemicsound.com/music/search` is a `POST` that is called after selecting a genre or mood, the body has the following:

```
POST /music/search HTTP/1.1
Content-Type: application/json; charset=utf-8
Host: agw.epidemicsite.com
Connection: close
User-Agent: Paw/3.2.2 (Macintosh; OS X/11.4.0) GCDHTTPRequest
Content-Length: 51

{"moods":[],"genres":["Funk"],"vocals":[],"page":1}
```

`/music/search` will return more than just tracks, please ignore moods/vocals/genres. The other fields are free for you to explore and implement as you see fit 🙏


### Guidelines

Tests are optional. The design/organization of the application code should be production ready.

The application should be runnable and working without major issues.

Ask any questions related to the implementation, but Stackoverflow and Google are your first stop for any obvious questions.

Please keep it simple, work in the details where it matters!

### FAQ

**Can I use frameworks/libraries?**

Yes.

**How much time should I spend?**

Aim for 4 😅, anything more than 8 hours is overdoing it.

**Does it need to play music?**

No.

**Do I need to care about vocals/sfx?**

No, just moods and genres.
