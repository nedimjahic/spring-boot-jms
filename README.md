# Requirements
- Build a prototype of a JMS listener, which should be connected to a foreign JMS broker
- Several users (10 - 20 users) may durable subscribe with different topics (at least 2 per user) to this foreign JMS broker and should consume messages as soon as these have been published to the appropriate topic
- This listener needs to keep connection and subscription over a long time period (months to years ), so it is important to report every interruption (either by JMS broker or by listener) and report as well the automated reconnection
- Report error messages during connection (unknown URL, unknown topic, wrong user resp. password, none unique clientID, ClientID already connected, etc..)
- The communication should be done by rest web services.
