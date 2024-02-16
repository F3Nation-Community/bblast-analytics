# Data Profile
## Volume
### Beatdowns
The average size of each beatdown ingested is 2.2 kb, however can range from 0.2kb to 7kb. The main contributor of space is the beatdown free text field, which can range. Every month results in about 9202 beatdowns which would be ~20mb a month of additional storage, .25 gb a year. 

## Velocity

### Beatdowns 
Beatdowns come in throughout an entire 24 hour period, however the ingestions are concentrated largely in the morning. Peaks at 7am.

#### Time of Day
![TimeOfDay](./What%20time%20are%20backblasts%20posted_%20(%20December%20)%20.png)

#### Day of Week
![DayOfWeek](./What%20day%20are%20backblasts%20posted_%20(%20December%20).png)

## Value
- Identify which AOs are growing, and which are flagging behind.
- Identify at which # beatdown someone is most likely stick with F3 versus quit.
- Identify which periods of the year attendance dips.
- Identify, by name, which Kotters to reach out to.

## Variety
- Beatdowns are ingested by both Paxminer and Slackblast, and after ingestion and fitted to the same schema.
- These tools have different code bases. 
Open question: What percentage of backblasts come through Paxminer versus coming through slackblast.

## Veracity
- Beatdowns are submitted by users, and there are some data controls but still much junk data is submitted. The goal in identifying these is to find out what guidelines we can put on the data collection tools that can improve data quality without making the barrier to submitting data too high. 
### Data Quality Problems ( Examples )
#### Count vs bd_attendance_count
When submitting a backblast, the count of PAX in attendance is submitted. The person submitting the backblast also tags all the pax in attendance. A user can either enter the count wrong, fail to tag some pax, or tag a pax that is not on slack. This leads to a situation where the count field in the backblasts doesn't match with the summation of all users in attendance. Open Question: Does slackblast have this same data quality problem?
- In January of 2024, there were 205 backblasts submitted in the St. Louis region ( not megaregion ). 20% of these, the attendance sum does not match the count

