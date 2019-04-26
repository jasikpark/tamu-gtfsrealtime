# tamu-gtfsrealtime
attempt to consume the a&amp;m bus api and provide a gtfsrealtime-compliant api

a&amp;m bus api: https://transport.tamu.edu/BusRoutesFeed/swagger/ui/index#!/Buses/Buses_GetBusesOnRoute_Mentor

so my plan is:

- [ ] work through the [rocket](https://rocket.rs) tutorial and documenation
- [ ] read through the [gtfs-realtime](https://github.com/google/transit/tree/master/gtfs-realtime/spec/en) spec in its entirety
- [ ] learn how to write an application that polls the api once every ten seconds (with some added random variance)
- [ ] learn how to work with databases so that there can be a single worker that polls the Spirit Bus api every ten seconds for updated info, that enters that information in a database for consumption
- [ ] take what I have learned from the [rocket](https://rocket.rs) tutorial and create a gtfs-realtime server

the program structure will be: 

- [ ] consume api from [a&amp;m bus api site](https://transport.tamu.edu/BusRoutesFeed/swagger/ui/index#!/Buses/Buses_GetBusesOnRoute_Mentor)
- [ ] store that in a clear, internal representation via meaningful rust structs
- [ ] create an api server that uses [rocket](https://rocket.rs) and serve that on a minimal vps
- [ ] implement a web-based administrative ui for the server

building on / resources&blog posts:

- [Legacy AVL system? It’s okay, join the club. | Kurt Raschke](https://kurtraschke.com/2015/01/legacy-avl-export/)
- [GitHub - kurtraschke/wmata-gtfsrealtime: GTFS-realtime StopTimeUpdate, VehiclePosition, and Alert feeds for WMATA](https://github.com/kurtraschke/wmata-gtfsrealtime)
- [GitHub - kurtraschke/septa-gtfsrealtime: GTFS-realtime for SEPTA TrainView and TransitView APIs.](https://github.com/kurtraschke/septa-gtfsrealtime)