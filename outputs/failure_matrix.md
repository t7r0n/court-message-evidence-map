# Failure Matrix: Court Message Evidence Map

| Scenario | Failure mode | Metric | Gate | Evidence |
| --- | --- | --- | --- | --- |
| people evidence replay | people_drift | people_coverage | block release until cited evidence is regenerated | ev_0000 |
| court operator packet | court_blindspot | court_latency | accept only if decision claims cite fixture evidence | ev_0007 |
| court operator packet | court_blindspot | court_latency | accept only if decision claims cite fixture evidence | ev_0011 |
| text-message regression harness | text-message_misroute | text-message_precision | open a regression issue with trace and benchmark delta | ev_0014 |
| preparing boundary probe | preparing_gap | preparing_risk | route to reviewer with evidence packet | ev_0021 |
| text-message regression harness | text-message_misroute | text-message_precision | open a regression issue with trace and benchmark delta | ev_0022 |
| people evidence replay | people_drift | people_coverage | block release until cited evidence is regenerated | ev_0028 |
