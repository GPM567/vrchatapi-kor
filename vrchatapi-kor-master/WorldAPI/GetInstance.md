# Get Instance With Tags
This API allows you to fetch an instance by passing the instanceid with tags from the world api or the user (location) api

## Request Method 
GET

## Endpoint
    https://api.vrchat.cloud/api/1/worlds/[ID]/[INSTANCEID]

id - the world id

instanceid - the world instance id 

(formatted like: number~accesstag(usr_number)~nonce(numbersandletters) or just number)
    
## Requires Authentication
Yes

## Returns 

Field | Type | Description
------|------|------------
id | string | Instance id with tags
name | String | Instance ID without tags
private | JSONArray | Private users (or false)
friends | JSONArray | Friend users (or false)
users | JSONArray | Users (or false)
hidden | string | if tag-hidden shows instance creator else null
nonce | string | shows the nonce from tags