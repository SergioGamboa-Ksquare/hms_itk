# Health Management System
# Final Project
## Sergio Gamboa

| Module   | Code |Description |
| ---------------- | :--: | ---: |
| Patient  |   interface patient{<br>id_patient: int;//easy identification<br> name_patient: string// identification;<br> email_patient:string//information<br> password_patient: string//Login info;<br>age_patient:  int//patient info; <br> gender_patient: string;//Some appointment would be necesary to know the gender <br>status_patient: boolean;//Served/Not served <br> status_new:boolena// New or not new |    This module is necessary beacause it will be the main user of the app, we need a way to identication, that provide us the main information about the user and a way to login into the system. |
| Doctor  | interface doctor{<br>id_doctor: int;//easy identification<br> name_doctor: string// identification;<br> email_doctor:string//information<br> password_doctor: string//Login info; <br> gender_doctor: string;//Some appointment would be necesary to know the gender <br>status_doctor: boolean;//Connected/disconnected <br>list_patient: list;//control of patients<br> number_patients: int;//control of patients<br> hours_available: int//control of appointment <br> schedule_doctor:list//To fix an appointment   <br> status_new:boolena// New or not new   | This module is important beacause the doctor will be able to give tha available hours and days, they will be able to see the active patients and a to put their status to answer a possible quickly contact  |
| Admin | interface admin{<br>id_admin: int;//easy identification <br> email_admin:string//information<br> password_admin: string//Login info;<br> list_new_patient:list;//To update patient list for doctors <br>list_status_patient: list;//to update list for doctors<p>list_new_doctor: list//To accept a new doctor  <p>list_status_doctor: list//To know doctors status  |      |
| Auth   | <br> Role based <br>Account creation Account authentication<br> JWT-based  |      |
| Contact  |     |      |
| Message  |     |      |
|  |     |     |

