# Project Plan

## Automatic Title Updater
- [ ] Create small Express server that will run locally and handle interacting with Beat Saber mod [HTTP Status](https://github.com/opl-/beatsaber-http-status/blob/master/protocol.md) and Twitch API.
- [ ] Use WebSockets to connect to localhost:6557/socket
- [ ] Connect to Twitch API
    - [ ] Handle programmatically fetching auth token
- [ ] Create listener for 'hello' event to get initial [Status Object](https://github.com/opl-/beatsaber-http-status/blob/master/protocol.md#status-object)
- [ ] Create listener for 'songStart' event that updates the stream title with the name of the song started
  - Ensure title length is less than 140 characters.

## Stream Visuals
- [ ] Spin up a simple React app that will be served locally
- [ ] Connect to localhost:6557/socket
- [ ] Combo HUD element
- [ ] Misses HUD element
- [ ] Score Multiplier HUD element
- [ ] Total Score HUD element
- [ ] Percentage Score HUD element
- [ ] Current Rating HUD element
- [ ] Energy Bar HUD element
- [ ] Song Timer HUD Element (*optional*)
- [ ] Animated Electric Combo visual that gains intensity as combo increases

## Misc
- [ ] Create single CLI command to spin up title updater and stream visuals locally
