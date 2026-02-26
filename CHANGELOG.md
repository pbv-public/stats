# Stats Schema Changelog

## [v2.2.0](https://github.com/pbv-public/stats/releases/tag/v2.2.0) on 2026-Feb-26
> * [Compare to Previous Version](https://github.com/pbv-public/stats/compare/v2.1.0...v2.2.0?expand=1)
> * Version Checksums: Functional=8280a25f9fdbe49411a5f495a58d0a68 Full=71596bd6f009b75a9c01a09168d221dc

- Added `team_kitchen_arrival` to player stats with team-level kitchen arrival stats (numerator/denominator counts for serving and returning roles, where both teammates had a fair opportunity to arrive at the kitchen)

-------------------------------------
## [v2.1.0](https://github.com/pbv-public/stats/releases/tag/v2.1.0) on 2025-Nov-12
> * [Compare to Previous Version](https://github.com/pbv-public/stats/compare/v2.0.0...v2.1.0?expand=1)
> * Version Checksums: Functional=88f8f339fa3d682e8542eba0e8676bee Full=77414163903bbb3691c1f5783c49e66a

- New structure, `kitchen_arrival_percentage`, with a new, improved algorithm for calculating the percentage of fair-chance kitchen arrivals.

-------------------------------------
## [v2.0.0](https://github.com/pbv-public/stats/releases/tag/v2.0.0) on 2025-Aug-07
> * [Compare to Previous Version](https://github.com/pbv-public/stats/compare/v1.4.1...v2.0.0?expand=1)
> * Version Checksums: Functional=85234ba31816641f701418262db0cd3b Full=e7048d44238f99d50cdabedcb22b3c83

- Multi-session videos support
- Most important change is in the URL structure, now it contains the session ID: instead of /{video_id}/stats.json it is now /{video_id}/{session_id}/stats.json, where session_id is 0-based index of the session in the video. Client can iterate through sessions using the session_id until it gets 404 Not Found.

-------------------------------------
## [v1.4.1](https://github.com/pbv-public/stats/releases/tag/v1.4.1) on 2025-Jul-14
> * [Compare to Previous Version](https://github.com/pbv-public/stats/compare/v1.4.0...v1.4.1?expand=1)
> * Version Checksums: Functional=d9fd7aa014c6e0a7373fb6b094d21ef0 Full=0b614be487264496c70924d986373547

- Docs updates: for the `kitchen_arrival` we specify that we consider only "rallies with at least 3 shots"

-------------------------------------
## [v1.4.0](https://github.com/pbv-public/stats/releases/tag/v1.4.0) on 2025-May-17
> * [Compare to Previous Version](https://github.com/pbv-public/stats/compare/v1.2.1...v1.4.0?expand=1)
> * Version Checksums: Functional=139ee6fae36b5c0902caab2915f024e0 Full=a16d60921c67122cf4b3fc37865619b1

- Running score properties moved to rallies[*].scoring_info.running_score, with server_number added for doubles games
- Added start_ms and end_ms timestamps to track shot duration for shots without the resulting_ball_movement
- Updated popup error definition with more specific criteria
- Changed description of average_x_coverage_percentage to clarify it's only relevant for doubles games, made it optional
- Added corrected boolean flag to worldPosition3D to indicate post-CV corrections

-------------------------------------
## [v1.2.1](https://github.com/pbv-public/stats/releases/tag/v1.2.1) on 2024-Nov-20
> * [Compare to Previous Version](https://github.com/pbv-public/stats/compare/v1.2.0...v1.2.1?expand=1)
> * Version Checksums: Functional=498f21cb9ce0163551e522ee46773a07 Full=fb3c186d85912eddbd4a208f4f9f85aa

- Back to the clean version of the schema

-------------------------------------
## [v1.2.0](https://github.com/pbv-public/stats/releases/tag/v1.2.0) on 2024-Nov-20
> * [Compare to Previous Version](https://github.com/pbv-public/stats/compare/v1.0.2...v1.2.0?expand=1)
> * Version Checksums: Functional=60e228b4f8ad7170a7322291cd5f4f4a Full=f17daeb3c89cedd71c173e37ce0a1223

- Back to the clean version of the schema

-------------------------------------
## [v1.0.2](https://github.com/pbv-public/stats/releases/tag/v1.0.2) on 2024-Nov-04
> * [Compare to Previous Version](https://github.com/pbv-public/stats/compare/v1.0.1...v1.0.2?expand=1)
> * Version Checksums: Functional=498f21cb9ce0163551e522ee46773a07 Full=fb3c186d85912eddbd4a208f4f9f85aa

- added `session` to indicate game vs. drill and how many participants

-------------------------------------
## [v1.0.1](https://github.com/pbv-public/stats/releases/tag/v1.0.1) on 2024-Sep-07
> * [Compare to Previous Version](https://github.com/pbv-public/stats/compare/v1.0.0...v1.0.1?expand=1)
> * Version Checksums: Functional=6e63a3da8d4e3954b373eab12276f5ec Full=ac5c40635576de3261cc15cec99eb5ce

- Added percentage of rallies won by length of rally for each team

-------------------------------------
## [v1.0.0](https://github.com/pbv-public/stats/releases/tag/v1.0.0) on 2024-Sep-03
> * [Compare to Previous Version](https://github.com/pbv-public/stats/compare/v1.0.0^...v1.0.0?expand=1)
> * Version Checksums: Functional=5e5e4a830c9b25b08607506f1418a141 Full=ed9d556b831bfb2730b28872cfb30bfa

- first release!
- share a ton of advanced stats for data lovers to peruse and analyze

