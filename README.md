# ColtureFit

[Heroku link][heroku] 

[heroku]: http://www.herokuapp.com

## Minimum Viable Product
-------------- 
ColtureFit is a web application inspired by ReverbNation and Sonicbids built using Ruby on Rails
and React.js to help musicians to connect with fans and book Gig at venues. ColtureFit allows users to:

<!-- This is a Markdown checklist. Use it to keep track of your progress! -->

- [ ] Create an account as a Fan, with additional capabilities as either a Band or Venue
- [ ] Log in / Log out
- [ ] Create, view, edit, and delete Bands or Venues if you sign up as either
- [ ] As a Band or Venue, create Gigs that Fans can keep up with
- [ ] Allow Bands to upload Albums, Songs, and Videos along with their EPK
- [ ] Search to find Bands/Gigs/Albums/Songs/Videos either by name, date released/performed/formed, genre or location
- [ ] Allow bands to apply for Gig at Venues 
- [ ] Have feed capabilities, where Fans can subscribe to Bands, Venues, or other Fans as well as objects

## Design Docs
* [View Wireframes][view]
* [DB schema][schema]

[view]: ./docs/views.md
[schema]: ./docs/schema.md

## Implementation Timeline

### Phase 1: User Authentication, JSON API, and Band/Fan/Venue/Album/Song/Video/Gig/Comment/Favorite/Reply/Image/message Model  (2 days)
In Phase 1, I will begin by implementing user signup and authentication using BCrypt. There will be a basic landing page after signup that will contain the container for the application's root React component. Users will sign up with email address and will choose whether they are a Band, a Venue or a Fan. If they are a Venue, they will have a Club with a Google map location and bio and an interface where they can choose Bands for Gigs or that Bands can submit their information to. A Band will have their full bio and will be able to display Albums, Songs, and Videos as well as have fans be able to subscribe to their feed (which will also have Gigs come up at existing Venues). A Fan will be any user (as Bands and Venues also can subscribe to each other) but would not have the capabilities of Bands or Venues, they would just be able to subscribe to Band/Venue feeds, other Fan feeds, Favorite Bands/Albums/Songs/Videos/Gigs  (which would then share it to their personal Feed) and post Comments. Only one Fan can be directly referred to as a Venue or Band. 

[Details][phase-one]

### Phase 2: Flux Architecture and Fan/Venue CRUD (2.5 days)
Phase 2 will begin by setting up Flux, the React Router and views for the main application. Stores will be needed for Fans which can also have membership of Bands or Venues (both of which probably don't need their own Store and all three of which will have CRUD functionality). Albums, Images, Press, Songs, Videos and Gigs will likely need their own stores as well, as most likely will Favorites and Comments. CRUD functionality will be needed for Albums (where you can take BandCamp, Soundcloud, Spotify, AudioMack, etc), Songs, Videos, Gigs and Comments while Favorites just need Create and Destroy functions. Once this is done, React views for the Fans, Venues, Albums, Songs, Videos and Gigs will have been created with full CRUD functionality that allows user-given information to be saved to the database. Bootstrap will be used to provide basic CSS styling.

[Details][phase-two]

### Phase 3: Band CRUD and View (2.5 days)
Phase 3 is the main meat of the website as the band is what is meant to ultimately drive traffic to the site. Band pages should have hooks for Twitter, Instagram and Facebook's API as should Venue pages. These sites double as EPKs so a band read page has to be laid out with Videos, Albums, Songs that are singles, their location, band images, short bio, genre, extended bio, discography, press, Gig calendar, Facebook/Twitter/Instagram APIs and Fans. Venues will also need to have a way to see the requests from bands that contact them, and bands should be able to see the venues that they contacted. Bands should be able to apply to Venues by clicking a link on the Venue page, sending them their EPK along with a brief message. Fans should also be able to message Venues, Bands and other Fans.

[Details][phase-three]

### Phase 4: Feed and search capabilities (2 days)
Phase 4 allow Fans to have feeds from different Bands and Venues. This means that a Fan can subscribe and get updates from Bands and Venues, and can also search by genre and location to discover new acts or places, songs, albums or
 (they can also additionally search by date for Gigs or songs/albums/videos). Favoriting (which will repost from a Fan's feed to their Fan's feeds), Commenting and Replying functionality will have been added by the end of this phase. 

[Details][phase-four]

### Phase 5: Styling Cleanup and Seeding (2 days)
Once the site is mostly built out, add more CSS, modals, transitions, and other things to generally make the site more attractive and user-friendly.  One of these things will be a cool index page that highlights various groups and Gigs that users can still sign in/up on.

[Details][phase-five]




[phase-one]: ./docs/phases/phase1.md
[phase-two]: ./docs/phases/phase2.md
[phase-three]: ./docs/phases/phase3.md
[phase-four]: ./docs/phases/phase4.md
[phase-five]: ./docs/phases/phase5.md
