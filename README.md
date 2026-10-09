# Bike trip routes

Live route data for Spoke. Riders ask for a ride; the app answers with time, distance, the stops between, and a map.

Edit `data/network.json` and commit to `main`. Open searches pick up the change within about 15 seconds. Bump `updatedAt` when you change the network.

## Shape

- `stops`: `id`, `name`, `area`, `lat`, `lng`
- `legs`: `from`, `to` (stop ids), `km`, `minutes`, `via` (street or trail)

Legs are two-way. Spoke picks the fastest chain of legs and draws those stops on the map.
