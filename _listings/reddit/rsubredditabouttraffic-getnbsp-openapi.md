---
swagger: "2.0"
x-collection-name: Reddit
x-complete: 0
info:
  title: Reddit Get Subreddit About Traffic
  description: Get the traffic for the current subreddit
  version: 1.0.0
host: www.reddit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '{/r/subreddit}/about/log':
    get&nbsp;:
      summary: Get Subreddit About Log
      description: Get a list of recent moderation actions.
      operationId: get&nbsp;RSubredditAboutLog
      x-api-path-slug: rsubredditaboutlog-getnbsp
      parameters:
      - in: query
        name: after
        description: fullname of a thing
        type: string
      - in: query
        name: before
        description: fullname of a thing
        type: string
      - in: query
        name: count
        description: 'a positive integer (default: 0)'
        type: string
      - in: query
        name: limit
        description: 'the maximum number of items desired (default: 25, maximum: 500)'
        type: string
      - in: query
        name: mod
        description: (optional) a moderator filter
        type: string
      - in: query
        name: show
        description: (optional) the string all
        type: string
      - in: query
        name: sr_detail
        description: (optional) expand subreddits
        type: string
      - in: query
        name: type
        description: one of (banuser, unbanuser, spamlink, removelink, approvelink,
          spamcomment, removecomment, approvecomment, addmoderator, invitemoderator,
          uninvitemoderator, acceptmoderatorinvite, removemoderator, addcontributor,
          removecontributor, editsettings, editflair, distinguish, marknsfw, wikibanned,
          wikicontributor, wikiunbanned, wikipagelisted, removewikicontributor, wikirevise,
          wikipermlevel, ignorereports, unignorereports, setpermissions, setsuggestedsort,
          sticky, unsticky, setcontestmode, unsetcontestmode, lock, unlock, muteuser,
          unmuteuser, createrule, editrule, deleterule, spoiler, unspoiler, modmail_enrollment,
          community_styling, community_widgets)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subreddit
      - About
      - Log
  '{/r/subreddit}/about/location':
    get&nbsp;:
      summary: Get Subreddit About Location
      description: Return a listing of posts relevant to moderators.
      operationId: get&nbsp;RSubredditAboutLocation
      x-api-path-slug: rsubredditaboutlocation-getnbsp
      parameters:
      - in: query
        name: after
        description: fullname of a thing
        type: string
      - in: query
        name: before
        description: fullname of a thing
        type: string
      - in: query
        name: count
        description: 'a positive integer (default: 0)'
        type: string
      - in: query
        name: limit
        description: 'the maximum number of items desired (default: 25, maximum: 100)'
        type: string
      - in: query
        name: location
        type: string
      - in: query
        name: only
        description: one of (links, comments)
        type: string
      - in: query
        name: show
        description: (optional) the string all
        type: string
      - in: query
        name: sr_detail
        description: (optional) expand subreddits
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subreddit
      - About
      - Location
  '{/r/subreddit}/about/where':
    get&nbsp;:
      summary: Get Subreddit About Where
      description: This endpoint is a listing.
      operationId: get&nbsp;RSubredditAboutWhere
      x-api-path-slug: rsubredditaboutwhere-getnbsp
      parameters:
      - in: query
        name: after
        description: fullname of a thing
        type: string
      - in: query
        name: before
        description: fullname of a thing
        type: string
      - in: query
        name: count
        description: 'a positive integer (default: 0)'
        type: string
      - in: query
        name: limit
        description: 'the maximum number of items desired (default: 25, maximum: 100)'
        type: string
      - in: query
        name: show
        description: (optional) the string all
        type: string
      - in: query
        name: sr_detail
        description: (optional) expand subreddits
        type: string
      - in: query
        name: user
        description: A valid, existing reddit username
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subreddit
      - About
      - Where
  /r/subreddit/about:
    get&nbsp;:
      summary: Get Subreddit About
      description: Return information about the subreddit.
      operationId: get&nbsp;RSubredditAbout
      x-api-path-slug: rsubredditabout-getnbsp
      responses:
        200:
          description: OK
      tags:
      - Subreddit
      - About
  /r/subreddit/about/edit:
    get&nbsp;:
      summary: Get Subreddit About Edit
      description: Get the current settings of a subreddit.
      operationId: get&nbsp;RSubredditAboutEdit
      x-api-path-slug: rsubredditaboutedit-getnbsp
      parameters:
      - in: query
        name: created
        description: one of (true, false)
        type: string
      - in: query
        name: location
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subreddit
      - About
      - Edit
  /r/subreddit/about/rules:
    get&nbsp;:
      summary: Get Subreddit About Rules
      description: Get the rules for the current subreddit
      operationId: get&nbsp;RSubredditAboutRules
      x-api-path-slug: rsubredditaboutrules-getnbsp
      responses:
        200:
          description: OK
      tags:
      - Subreddit
      - About
      - Rules
  /r/subreddit/about/traffic:
    get&nbsp;:
      summary: Get Subreddit About Traffic
      description: Get the traffic for the current subreddit
      operationId: get&nbsp;RSubredditAboutTraffic
      x-api-path-slug: rsubredditabouttraffic-getnbsp
      responses:
        200:
          description: OK
      tags:
      - Subreddit
      - About
      - Traffic
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---