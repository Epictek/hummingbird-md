# hummingbird.me markdown v1

Hummingbird is awesome blah blah blah

[Official docs](https://www.mashape.com/vikhyat/hummingbird-v1).

Endpoint: https://hummingbirdv1.p.mashape.com

Following are the available functions.

...

# Anime
Provides basic information on the specified anime, such as its status (Currently/Finished airing), url, alt title and genres.

## Request
````
GET /anime/{anime-slug}
````

# Authenticate
Get a user's authentication token, using the password and either one of the username and email.

## Request
````
GET /users/authenticate/
    [?email={username}]
    ?password={password}
    [?username={username}]
````

# Library
Get a user's library entries in a given section.

## Request
````
GET /users/{username}/library
    ?auth_token={auth_token}
    ?status={status}
````

#Library Remove
Remove an entry from the user's library

## Request

````
GET /libraries/{anime_id}/remove
    ?auth_token={auth_token}
````

#Library Update
Create or update an entry in a user's library

## Request
````
GET /libraries/{anime_id}
    ?auth_token={auth_token}
    [?episodes_watched={}]
    [?increment_episodes={}]
    [?notes={}]
    [?privacy={}]
    [?rating={}]
    [?rewatched_times={}]
    [?status={}]
````
