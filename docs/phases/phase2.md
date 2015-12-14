# Phase 2: Flux Architecture and Fan/Venue CRUD (2.5 days)

## Rails
### Models

### Controllers

### Views

## Flux
### Views (React Components)
* FanIndex
  - Feed
  - Messages
  - Fan Name
  - Recent Comments by Fan
  - Fan Pictures
  - Short Fan Bio
  - Extended Fan Bio
  - Links
  - Show Calendar 
  - Favorited Items
  - Twitter/FB/Instagram API Display
  - Search Bar (+ link to menu)
* VenueIndex
 - Feed
 - Messages
 - Venue Name
 - Band Requests (visible to Venue only)
 - Venue Pictures
 - Short Venue Bio
 - Links
 - Extended Venue Bio
 - Google Maps location
 - Twitter/FB/Instagram API Display
 - Venue Calendar
 - Recent Comments by Venue
 - Favorited Items
 - Search Bar (+ link to menu)



### Stores
* Fan
* Band
* Venue
* Album
* Song
* Video
* Gig
* Comment
* Favorite
* Reply
* PressItem
* Image

### Actions0
-> triggered by ApiUtil
* ApiActions.receiveAllFans -> triggered by ApiUtil
* ApiActions.receiveSingleFan
* ApiActions.receiveAllBands
* ApiActions.receiveSingleBand
* ApiActions.receiveAllVenues
* ApiActions.receiveSingleVenue
* ApiActions.receiveAllAlbums
* ApiActions.receiveSingleAlbum
* ApiActions.receiveAllSongs
* ApiActions.receiveSingleSong
* ApiActions.receiveAllVideos
* ApiActions.receiveSingleVideo
* ApiActions.receiveAllGigs
* ApiActions.receiveSingleGig
* ApiActions.receiveAllComments
* ApiActions.receiveSingleComment
* ApiActions.receiveAllMessagesForUser
* ApiActions.receiveSingleMessage
* ApiActions.receiveAllPressForUser
* ApiActions.receiveSinglePressItem
* ApiActions.receiveAllImagesForUser
* ApiActions.receiveSingleImage

 -> triggers ApiUtil
* FanActions.fetchAllFans
* FanActions.fetchSingleFan
* FanActions.createFan
* BandActions.fetchAllBands
* BandActions.fetchSingleBand
* BandActions.createBand
* BandActions.editBand 
* BandActions.destroyBand
* VenueActions.fetchAllVenues
* VenueActions.fetchSingleVenue
* VenueActions.createVenue
* VenueActions.editVenue 
* VenueActions.destroyVenue.
* AlbumActions.fetchAllAlbums
* AlbumActions.fetchSingleAlbum
* AlbumActions.createAlbum
* AlbumActions.editAlbum
* AlbumActions.destroyAlbum
* SongActions.fetchAllSongs
* SongActions.fetchSingleSong
* SongActions.createSong
* SongActions.editSong
* SongActions.destroySong
* VideoActions.fetchAllVideos
* VideoActions.fetchSingleVideo
* VideoActions.createVideo
* VideoActions.editVideo
* VideoActions.destroyVideo
* GigActions.fetchAllGigs
* GigActions.fetchSingleGig
* GigActions.createGig
* GigActions.editGig
* GigActions.destroyGig
* CommentActions.fetchAllComments
* CommentActions.fetchSingleComment
* CommentActions.createComment
* CommentActions.editComment
* CommentActions.destroyComment
* ReplyActions.fetchAllReplies
* ReplyActions.fetchSingleReply
* ReplyActions.createReply
* ReplyActions.editReply
* ReplyActions.destroyReply
* AlbumActions.fetchAllFavorites
* AlbumActions.fetchSingleFavorite
* AlbumActions.createFavorite
* AlbumActions.destroyFavorite
* MessageAction.fetchAllMessagesForUser
* MessageActions.fetchSingleMessage
* MessageActions.createMessage
* MessageActions.destroyMessage
* PressActions.fetchAllPressForUser
* PressActions.fetchSinglePressItem
* PressActions.createPressItem
* PressActions.destroyPressItem
* ImageActions.fetchAllImagesForUser
* ImageActions.fetchSingleImage
* ImageActions.createImage
* ImageActions.destroyImage


### ApiUtil
* ApiUtil.fetchAllFans
* ApiUtil.fetchSingleFan
* ApiUtil.createFan
* ApiUtil.destroyFan
* ApiUtil.fetchAllBands
* ApiUtil.fetchSingleBand
* ApiUtil.createBand
* ApiUtil.editBand
* ApiUtil.destroyBand
* ApiUtil.fetchAllVenues
* ApiUtil.fetchSingleVenue
* ApiUtil.createVenue
* ApiUtil.editVenue
* ApiUtil.destroyVenue
* ApiUtil.fetchAllAlbums
* ApiUtil.fetchSingleAlbum
* ApiUtil.createAlbum
* ApiUtil.editAlbum
* ApiUtil.destroyAlbum
* ApiUtil.fetchAllSongs
* ApiUtil.fetchSingleSong
* ApiUtil.createSong
* ApiUtil.editSong
* ApiUtil.destroySong
* ApiUtil.fetchAllVideos
* ApiUtil.fetchSingleVideo
* ApiUtil.createVideo
* ApiUtil.editVideo
* ApiUtil.destroyVideo
* ApiUtil.fetchAllGigs
* ApiUtil.fetchSingleGig
* ApiUtil.createGig
* ApiUtil.editGig
* ApiUtil.destroyGig
* ApiUtil.fetchAllComments
* ApiUtil.fetchSingleComment
* ApiUtil.createComment
* ApiUtil.editComment
* ApiUtil.destroyComment
* ApiUtil.fetchRepliesForPost
* ApiUtil.fetchSingleReply
* ApiUtil.createReplyForPost
* ApiUtil.editReply
* ApiUtil.destroyReply
* ApiUtil.fetchFavoritesForPost
* ApiUtil.fetchSingleFavorite
* ApiUtil.createFavoriteForPost
* ApiUtil.deleteFavorite
* ApiUtil.fetchMessagesForUser
* ApiUtil.fetchSingleMessage
* ApiUtil.createMessage
* ApiUtil.destroyMessage
* ApiUtil.fetchPressForUser
* ApiUtil.fetchSinglePressItem
* ApiUtil.createPressItem
* ApiUtil.destroyPressItem
* ApiUtil.fetchImagesForUser
* ApiUtil.fetchSingleImage
* ApiUtil.createImage
* ApiUtil.destroyImage


## Gems/Libraries
* Flux Dispatcher (npm)
* Twitter Bootstrap
