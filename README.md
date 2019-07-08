# intro_to_NoSQL

There are two part in this assignment:
1. Simple social model and topics in Neo4j 
- Load baseball data from neo4j database which includes
-- Node Labels:

-- Team: Core information loaded from Lahman 2017
--- Player: Core information loaded from Lahman 2017
--- Fan: New entity representing a baseball fan.
--- Comment: A Fan made a comment on a team or player.
-- Relationships:
--- Appeared: Represents the fact that a player "appeared" for a team in a year. Loaded from a small subset of Lahman 2017.
--- Supports: A Fan supports a Team
--- Follows: A Fan follows (the comments of) another Fan.
--- CommentOn: Represents the relationship between a Comment and a Team/Player.
--- CommentBy: Relationship between a Fan and Comment.
--- ResponseTo: Indicates that a Comment is a ResponseTo a Comment.
- Implement and test the following methods:
-- find_nodes_by_template
-- create_fan
-- get_fan
-- create_player
-- get_player
-- create_team
-- get_team
-- create_supports
-- get_appearance
-- create_appearance_all
-- create_follows
-- get_comment
-- create_comment
-- create_sub_comment
-- get_sub_comments
-- get_player_comments
-- get_team_comments
-- get_players_by_team

2. Add API result cache for database query results using Redis.
