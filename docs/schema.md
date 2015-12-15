# Schema Information

## fan
   column name | data type | details
---------------|-----------|-----------------------
id             | integer   | not null, primary key
email          | string    | not null, indexed, unique
username       | string    | not null, indexed
password_digest| string    | not null
session_token  | string    | not null, indexed
short_bio      | string    | 
long_bio       | text      | 
location_zip   | integer   | not null
account_type   | string    | not null, indexed, inclusion in %w(fan band venue)

## band
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
fan_id      | integer   | not null, foreign key (references fans), indexed, unique
discography | text      |
genre       | text      | not null, indexed
members     | text      |

## venue
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
fan_id      | integer   | not null, foreign key (references fans), indexed, unique
geo_lat     | decimal   |
geo_lng     | decimal   |
address     | string    |

## album
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
band_id     | integer   | not null, foreign key (references bands), indexed
title       | string    | not null, indexed
long_bio    | text      |
date_made   | datetime  | not null, indexed
link_src    | string    | 

## song 
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
band_id     | integer   | not null, foreign key (references fans), indexed
album_id    | integer   | foreign key (references albums), indexed
title       | string    | not null, indexed
long_bio    | text      |
date_made   | datetime  | not null, indexed
link_src    | string    | 

## video
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
band_id      | integer   | not null, foreign key (references fans), indexed
album_id    | integer   | foreign key (references albums), indexed
title       | string    | not null, indexed
long_bio    | text      |
date_made   | datetime  | not null, indexed
link_src    | string    | 


## image
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
fan_id      | integer   | not null, foreign key (references fans), indexed
title       | string    | 
long_bio    | text      |
date_made   | datetime  |
link_src    | string    | 

## press 
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
fan_id      | integer   | not null, foreign key (references fans), indexed
title       | string    | not null
publisher   | string    | not null
body        | text      | not null
date_made   | datetime  |
link_src    | string    | 

## gig
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
venue_id    | integer   | not null, foreign key (references venues), indexed
title       | string    | not null, indexed
date        | datetime  | not null, indexed
description | text      | not null

## booked_act
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
band_id     | integer   | not null, foreign key (references bands), indexed
gig_id    | integer   | not null, foreign key (references gigs), indexed


## favorite
column name | data type | details
------------|-----------|-----------------------
id            | integer   | not null, primary key
liking_user_id| integer   | not null, foreign key (references fans), indexed
liked_user_id | string    | not null, foreign key (references fans), indexed


## comment
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
fan_id      | integer   | not null, foreign key (references fans), indexed
title       | string    | not null
body        | text      | not null

## reply
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
fan_id      | integer   | not null, foreign key (references fans), indexed
item_id     | integer   | not null, foreign key (references item)
body        | text      | not null

## message
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
fan _id     | integer   | not null, foreign key (references fans), indexed
title       | string    | not null
body        | text      | not null

