cooki-api
=========

First Header                                    | Second Header 
----------------------------------------------- | ------------- 
GET /users/sing_in                              | Sign in  
GET /users/sing_up                              | Sign up
GET /users/[id or me]                           | User
GET /users/[id or me]/chip_feeds                | User's Chip Feed
GET /users/[id or me]/crew_collections          | User's Crew Collections
GET /users/[id or me]/following_collections     | User's Following Collections
GET /news_feeds                                 | News Feeds
GET /categories/[name]                          | Category
GET /categories/[name]/category_feeds           | Category Feeds
GET /collections/[id]                           | Collection
GET /collections/[id]/collection_feeds          | Collection Feeds
GET /nodes/[id]                                 | Node Show
GET /nodes/[id]/comments                        | Comments
POST /nodes/[id]/comments                       | Create a new comment
DELETE /nodes/[id]/comments                     | Delete a comment
GET /nodes/[id]/chips                           | Chips
POST /nodes/[id]/chips                          | Create a new chip
POST /friend_requests/[target user id]          | Send friend request
