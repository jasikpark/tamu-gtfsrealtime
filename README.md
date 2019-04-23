# tamu-gtfsrealtime
attempt to consume the a&amp;m bus api and provide a gtfsrealtime-compliant api

a&amp;m bus api: https://transport.tamu.edu/BusRoutesFeed/swagger/ui/index#!/Buses/Buses_GetBusesOnRoute_Mentor

so the plan is:

- [ ] consume api from [a&amp;m bus api site](https://transport.tamu.edu/BusRoutesFeed/swagger/ui/index#!/Buses/Buses_GetBusesOnRoute_Mentor)
- [ ] store that in a clear, internal representation via meaningful rust structs
- [ ] create an api server that uses [rocket](https://rocket.rs) and serve that on a minimal vps

building on / resources&blog posts:

- [Legacy AVL system? It’s okay, join the club. | Kurt Raschke](https://kurtraschke.com/2015/01/legacy-avl-export/)
- [GitHub - kurtraschke/wmata-gtfsrealtime: GTFS-realtime StopTimeUpdate, VehiclePosition, and Alert feeds for WMATA](https://github.com/kurtraschke/wmata-gtfsrealtime)
- [GitHub - kurtraschke/septa-gtfsrealtime: GTFS-realtime for SEPTA TrainView and TransitView APIs.](https://github.com/kurtraschke/septa-gtfsrealtime)