cooki-api
=========

First Header                                    | Second Header 
----------------------------------------------- | ------------- 
GET /users/sing_in                              | Sign in  
GET /users/sing_up                              | Sign up
GET /users/[id or me]                           | User
GET /users/[id or me]/crew_collections          | User's Crew Collections
GET /users/[id or me]/following_collections     | User's Following Collections
GET /news_feeds                                 | News Feeds
GET /nodes/[id]                                 | Node Show
GET /nodes/[id]/comments                        | Comments
POST /nodes/[id]/comments                       | Create a new comment
DELETE /nodes/[id]/comments                     | Delete a comment
GET /nodes/[id]/chips                           | Chips
POST /nodes/[id]/chips                          | Create a new chip


### User

```
{
"name": "Siwon Choi",
"id": 4,
"description": "",
"email": "siwonred@gmail.com",
"chips": "72.0",
"image_thumb": "https://cooki-jp.s3.amazonaws.com/users/images/4/thumb/398769_2589222609734_433718147_n.jpeg?1346068708",
"image_list": "https://cooki-jp.s3.amazonaws.com/users/images/4/list/398769_2589222609734_433718147_n.jpeg?1346068708",
"image_profile": "https://cooki-jp.s3.amazonaws.com/users/images/4/profile/398769_2589222609734_433718147_n.jpeg?1346068708",
"nodes_count": 84,
"crew_collections_count": 19,
"following_collections_count": 62,
"friends_count": 15,
"chip_feeds_count": 542,
"is_friend": false,
"sent_friend_request": null,
"received_friend_request": null,
"notifications_count": 2
}
```


### User's Collections

```
[
{
"id": 16,
"name": "Bugs",
"user_id": 18,
"scope": "public",
"description": "",
"is_crew": true,
"is_following": false,
"is_invited": false,
"nodes_count": 279,
"crews_count": 291,
"followers_count": 1,
"category_name": "Inside Cooki",
"cover_image_grid": "https://cooki-jp.s3.amazonaws.com/collections/cover_images/16/grid/open-uri20120810-13162-13azh4r.?1349685046",
"cover_image_profile": "https://cooki-jp.s3.amazonaws.com/collections/cover_images/16/profile/open-uri20120810-13162-13azh4r.?1349685046",
"cover": {
"id": 699,
"kind": null,
"link_title": "",
"message_formatted": "<p>도모군</p>",
"source": "Bake It",
"cover_image_geometry_tile": "394x333",
"video_link": null,
"user": {
"id": 22,
"name": "Nicole Choung",
"image_thumb": "https://cooki-jp.s3.amazonaws.com/users/images/22/thumb/stringio.txt?1344604163"
}
},
"user": {
"id": 18,
"name": "Paul 'Sungyoung' Jung",
"image_thumb": "https://cooki-jp.s3.amazonaws.com/users/images/18/thumb/stringio.txt?1346652907"
}
},
{…}
]
``` 