# tamu-gtfsrealtime
attempt to consume the a&amp;m bus api and provide a gtfsrealtime-compliant api

a&amp;m bus api: https://transport.tamu.edu/BusRoutesFeed/swagger/ui/index#!/Buses/Buses_GetBusesOnRoute_Mentor

so the plan is:

- [ ] consume api from [a&amp;m bus api site](https://transport.tamu.edu/BusRoutesFeed/swagger/ui/index#!/Buses/Buses_GetBusesOnRoute_Mentor)
- [ ] store that in a clear, internal representation via meaningful rust structs
- [ ] create an api server that uses [rocket](https://rocket.rs) and serve that on a minimal vps