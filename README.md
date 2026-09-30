# LifeMap public static transit pack development sample

This repository hosts **public, user-independent test data** for the LifeMap LM-084 Structured Transit development spike. It contains no user Raw Location, user journey endpoints, photos, account state or analytics. LifeMap requests a coarse region pack and resolves individual journeys on device. The hosting URL is a replaceable input to its Resource Provider, not part of Train/Flight routing logic.

## Shanghai Maglev 2026-09-28 sample

`shanghai-maglev-20260928.json` (7,363 bytes; SHA-256 `97001c1b6e7cf6b6fbf752652a9bb58e4044c4b61d118f24b7ed373d3ccbe59e`) is a small, versioned static route sample. It contains two ordered public passenger Maglev route relations and their Longyang Road/Pudong Airport stops. The route is **Inferred geometry only**; the pack never proves a particular user's boarding, train, service, date or recorded location. This sample alone is not complete Shanghai transit coverage.

Source: [Geofabrik Shanghai OpenStreetMap extract dated 2026-09-28](https://download.geofabrik.de/asia/china/shanghai-260928.osm.pbf), source SHA-256 `0d079141db0b3ddb338484fc8293846f0664cc03b15d554082b59a0d6d407fe2`. Passenger-service cross-check: [Shanghai municipal government transport page](https://english.shanghai.gov.cn/en-Transportation/20240102/44f499a17b324b25996f2d58fcbf5f23.html). The pack embeds source, license and attribution metadata.

**License and attribution:** contains data © OpenStreetMap contributors, available under the [Open Database License 1.0 (ODbL)](https://opendatacommons.org/licenses/odbl/1-0/). See [OpenStreetMap copyright and attribution](https://www.openstreetmap.org/copyright). The JSON is available in machine-readable form under the same data license. LifeMap must display appropriate OpenStreetMap attribution when showing a route derived from this pack.

This is a zero-cost development distribution mechanism. The production Resource Provider can use a different host without changing the Train/Flight resolver.
