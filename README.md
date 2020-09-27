# SBRC 2019 dataset


## Dataset description

The dataset is a CSV file, where each line represents a participant and the time he enters in a given session. Each line has 5 columns (timestamp, ts, id, inst_id) where each column indicates the time that a participant enters in a session, the technical session, the participant's id, and the participant's institution id, respectively.

## Collection environment

The data was collected by a gamification system, at the 37th edition of the SBRC, a network and distributed systems conference that took place at Gramado-RS, Brazil. 
The conference was composed of Technical Sessions, Workshops, Keynotes, and other secondary events, where each event participation (for example, enter a session, asking questions) had different points.

## Data collection methodology

The event attendees received badges with unique QR codes scanned by the local organization team through iOS/Android apps. The QR code scanning process allowed registering when participants entered a  room where some technical session was happening, and the questions asked. We did not record when an attendee left the room.  
After the QR  scanning process, the attendees’ data was sent to a web server, which validated the data against gamification’s rules and consolidated the attendees’ scores. Leader boards placed around the convention center displayed top-n scores for attendees and institutions. It is important to highlight that the participation in the gamification was optional, that is, a participant could ask to be removed from the system or not to have its QRCode scanned.
