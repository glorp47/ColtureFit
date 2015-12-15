# Phase 1: User Authentication, JSON API, and Band/Fan/Venue/Album/Song/Video/Gig/Comment/Favorite/Reply/Message Model  (2 days)

## Rails
### Models
* Fan
* Band
* Venue
* Gig
* Press Item
* Image
* Album
* Song
* Video
* Comment
* Favorite
* Reply
* Message


### Controllers
* FanController (create, index, new)
* SessionsController (create, new, destroy)
* BandController (create, new, index, show, update)
* VenueController (create, new, index, show, update)
* Api::GigController (create, new, index, show, update)
* Api::AlbumController (create, new, index, show, update)
* Api::SongController (create, new, index, show, update)
* Api::VideoController (create, new, index, show, update)
* Api::CommentController (create, new, index, show, update)
* Api::FavoriteController (create, new, index, show, update)
* Api::ReplyController (create, new, index, show, update)
* Api::MessageController (create, new, show, destroy)
* Api::ImageController (create, new, show, update, destroy)

### Views
* fans/new.html.erb
* session/new.html.erb
* fans/index.json.jbuilder
* fans/show.json.jbuilder
* bands/index.json.jbuilder
* bands/show.json.jbuilder
* venues/index.json.jbuilder
* venues/show.json.jbuilder
* bands/index.json.jbuilder
* bands/show.json.jbuilder
* gigs/index.json.jbuilder
* gigs/show.json.jbuilder
* albums/index.json.jbuilder
* albums/show.json.jbuilder
* songs/index.json.jbuilder
* songs/show.json.jbuilder
* videos/index.json.jbuilder
* videos/show.json.jbuilder
* comments/index.json.jbuilder
* comments/show.json.jbuilder
* messages/index.json.jbuilder
* messages/show.json.jbuilder
* images/show.json.jbuilder

## Flux
### Views (React Components)

### Stores

### Actions

### ApiUtil

## Gems/Libraries
* BCrypt (Gem)
