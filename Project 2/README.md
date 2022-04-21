# Investigate a Dataset - NoShow Appointments Dataset
## by Pranav Medhi


## NoShow Appointments Dataset

> This dataset collects information
from 100k medical appointments in
Brazil and is focused on the question
of whether or not patients show up
for their appointment. A number of
characteristics about the patient are
included in each row.
●‘ScheduledDay’ tells us on
what day the patient set up their
appointment.
● ‘Neighborhood’ indicates the
location of the hospital.
● ‘Scholarship’ indicates
whether or not the patient is
enrolled in Brasilian welfare
program Bolsa Família.
● Be careful about the encoding
of the last column: it says ‘No’ if
the patient showed up to their
appointment, and ‘Yes’ if they
did not show up.



## Summary of Findings

#### The following partial conclusions can be put forth from the research done above:

- There was a minor difference between the not showing up proportions of Male vs Female. So, only gender is not a valid parameter for making any conclusions about the dataset.
- The not-showing up rate for the teenagers(0-18) and the pre-adult(18-37) ages was the highest among the age-groups. A little idea from this result we got was that the higher the age more the probability of showing up on any given appointment.
- Upon further research into the Aged age-group (55,115) an observation that the females of the aged group had a slightly higher probability of not showing up than their male counterparts.
- SMS received was one of the parameters where we found some clear differences. We observed that SMS not received and still showing up was pretty high probability leading to the conclusion that receiving or not receiving an SMS was not so much of a factor for not showing up.
- After comparing the not-showing up probabilities of all the disorders ,it can be concluded that Alcoholism lead to the most missed appointments compared to other disorders.

#### Limitations
- We didnt consider the different levels of Handicap because of smaller dataset size for them. It could be affecting the overall dataset.
- We didnt consider the scheduledday and appointmentDay columns , but it could be a possibility that majority of the patients might not have showed up on a certain day , because of some natural disaster that might have taken place. 