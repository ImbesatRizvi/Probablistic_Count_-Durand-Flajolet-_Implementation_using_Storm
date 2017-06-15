# Probablistic_Count_Implementation_using_Storm
Stream processing of meetup.com streams for probabilistic counting by Durand-Flajolet algorithm using Apache Storm

Implementation as part of the Scalable System for Data Science Course at Department of Computational and Data Sciences (CDS), Indian Institute of Science (IISc), Bangalore, India.

Streams of data can be processed for the purpose of distinct or unique count of field enteries which can be of interest to us. This nature of problem is referred to as
“Counting distinct elements in a stream”. The data processed for the course was for meetup.com RSVP (https://www.meetup.com/meetup_api/docs/stream/2/rsvps/) and EVENT (https://www.meetup.com/meetup_api/docs/stream/2/open_events/) streams.

The StreamGenSpount.java file generates the streams to be processed from saved json data obtained from above mentioned streaming api. The FieldCountBolt.java is where the implemetation of Durand-Flajolet (http://algo.inria.fr/flajolet/Publications/DuFl03.pdf) algorithm is carried out.