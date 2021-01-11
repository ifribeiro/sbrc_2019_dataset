# dataset description

The dataset is a CSV file, where each line represents the participant interaction in the session. Each line has 5 columns (Name, Institution, session, participation, updated_at) where each column indicates participants' name, his institution, the session he enters, the type of participation, and the time that the interaction occurs.

There are two types of participation:
- Join: when a participant enters in a session
- Question: when a participant is in a session and asks a question

# collection environment

The data was collected by a gamification system, at the 37th edition of the SBRC, a network and distributed systems conference that took place at Gramado-RS, Brazil. 
The conference was composed of Technical Sessions, Workshops, Keynotes, and other secondary events, where each event participation (for example, enter a session, asking questions) had different points.

# data collection methodology

The event attendees received badges with unique QR codes scanned by the local organization team through iOS/Android apps. The QR code scanning process allowed registering when participants entered a  room where some technical session was happening, and the questions asked. We did not record when an attendee left the room.  
After the QR  scanning process, the attendees’ data was sent to a web server, which validated the data against gamification’s rules and consolidated the attendees’ scores. Leader boards placed around the convention center displayed top-n scores for attendees and institutions. It is important to highlight that the participation in the gamification was optional, that is, a participant could ask to be removed from the system or not to have its QRCode scanned.

# trace description

The trace for the one simulator (file sbrc_2019.txt) generated from the dataset, represents a sequence of connections and disconnections that happened along the the 2nd, 3th and 4th day of the event.

The first column is the time when the event (connection or disconnection) happened, second column is a command that will be used for the one simulator, the third and fourth columns represents two distinct nodes that will be connected or disconnected and the last column indicates if either a connection (up) or disconnection (down) should de made for that two nodes.