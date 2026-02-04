# Doctor\_appointment\_backend

🏥 System Overview: Doctor Appointment ER Diagram

Doctor Appointment Backend

&nbsp;- The ER diagram models the complete lifecycle of a medical consultation,

&nbsp;  from booking an appointment to consultation, payment, communication,

&nbsp;  and feedback.



Core Design

&nbsp;- The Appointment entity is the central entity of the system.

&nbsp;- All major functionalities such as booking, payment, chat, feedback,

&nbsp;  and medical records depend on an appointment.



Key Relationships

\- A Patient can book multiple Appointments, but each Appointment

&nbsp; must be linked to exactly one Patient.



\- A Doctor can attend multiple Appointments, but an Appointment

&nbsp; cannot exist without a Doctor.



\- A Hospital employs multiple Doctors, forming a one-to-many relationship.



Weak Entity

&nbsp;    - Patient\_record is modeled as a weak entity because medical records

&nbsp;      do not have meaning without an Appointment.

&nbsp;    - It is identified through the Appointment using an identifying relationship.



Supporting Features

&nbsp; - Payment is linked one-to-one with Appointment and is optional

&nbsp;   to support paid, pending, or refunded cases.



&nbsp; - Chat allows multiple messages per Appointment to enable

&nbsp;   doctor-patient communication.



&nbsp; - Feedback is collected after consultation and is optional.



&nbsp; - Notification supports reminders, cancellations, and re-engagement

&nbsp;   messages for Patients.



Design Outcome

&nbsp;- The ER design correctly applies cardinality, participation constraints,

&nbsp;  and weak entities to maintain data integrity and scalability.



&nbsp; 

