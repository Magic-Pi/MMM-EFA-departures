# MMM-EFA-departures
MagicMirror² module to show departures for public transport stations using the EFA system.

Station IDs can be found here for example:
http://www.eg-blog.de/?p=822

Configuration for Düsseldorf HBF/Main Station:
		{
			module: 'MMM-EFA-departures',
			position: 'top_right',
			config: {
				efaUrl: "http://efa.vrr.de/standard/XSLT_DM_REQUEST",
				stopID: "20018235",
				stopName: "Loading station name …",
				lines: ['all'],
				maxDepartures: 4,
				reload: 1 * 60 * 1000,
				toggleDepTime: true,
				toggleDepTimePerReload: 6, //Every 10 seconds
				fade: true,
				fadePoint: 0.25 // Start on 1/4th of the list.			
			}
		},

API-Endpoints (EfaUrl):

Verkehrsverbund Rhein-Ruhr

http://efa.vrr.de/standard/XSLT_DM_REQUEST

Verkehrs- und Tarifverbund Stuttgart GmbH

http://www2.vvs.de/vvs/XSLT_DM_REQUEST

traveline south east: Journey Planner

http://www.travelinesoutheast.org.uk/se/XSLT_DM_REQUEST

MVV

http://efa.mvv-muenchen.de/mobile/XSLT_DM_REQUEST

Ding.EU

http://www.ding.eu/mobile/ding2/XSLT_DM_REQUEST
