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

# News Feeds
```
{
"since": {
"created_at": "2012-10-15T01:07:50Z",
"id": 600197
},
"feeds": [
{
"bind_type": null,
"bind": null,
"node": {
"id": 8584,
"scope": "news",
"status": "published",
"extra_type": null,
"lang": "ko",
"ref_type": "Post",
"created_at": "2012-10-15T06:14:31Z",
"num_pageviews": 9,
"ref": {
"id": 8277,
"kind": "readability",
"link_title": "(101) Firing: How do you fire an employee that just isn't good enough? - Quora",
"message_formatted": "<p>완벽한 하이어링에 꼭 필요한 것이, 효과적인 해고인 것 같습니다. 그러면서도 정말 어려운 일이네요.</p>\n\n<p>쿼라에 올라온 여러 경험담/조언들을 보자면 결국 케바케이고, 해고해야 할 직원이 어떤 타입이고 어떤 상황에 처해있는지에 따라 모두 다르게 접근해야 한다는 부분이 핵심인 것 같습니다.</p>\n\n<p>Dividers(구성원들 사이에 광범위하게 악영향을 끼치는 사람, 예: 정치적인 행동으로 팀웍을 떨어트리는 사람) 와 Subtractors (그냥 퍼포먼스가 떨어지는 구성원) 로 먼저 구분하는 것이 우선이며, 이에 따른 접근이 달라야 한다는 말입니다. </p>\n\n<p>번역중 (..)</p>",
"source": "Bake It",
"cover_image_geometry_tile": "394x185",
"video_link": null,
"chips_count": 0,
"cover_image": "https://cooki-jp.s3.amazonaws.com/posts/cover_images/8277/tile/open-uri20121015-17445-iusrwk.?1350281853",
"link": "/nodes/8584/link",
"link_zoom": "/nodes/8584#zoom",
"link_origin": "http://www.quora.com/Firing/How-do-you-fire-an-employee-that-just-isnt-good-enough",
"link_domain": "Quora",
"is_zoom": true,
"created_at": "2012-10-15T06:14:31Z",
"user": {
"id": 18,
"name": "Paul 'Sungyoung' Jung",
"image_thumb": "https://cooki-jp.s3.amazonaws.com/users/images/18/thumb/stringio.txt?1346652907"
},
"collection": {
"id": 193,
"name": "Pursuit of Perfect Hiring",
"user_id": 18,
"is_crew": false,
"is_following": true
},
"comments": [],
"chips": []
}
}
}, {}
}
```