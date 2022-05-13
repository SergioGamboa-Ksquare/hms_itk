# Health Management System
# Final Project
## Sergio Gamboa

| Module   | Code |Description |
| ---------------- | :--: | ---: |
| Patient  | <pre>```ts interface patient
{
    id_patient: int;//easy identification
    name_patient: string// identification;
    email_patient:string//information
    password_patient: string//Login info;
    age_patient:  int//patient info;
    gender_patient: string;//Some appointment would be necesary to know the gender
    status_patient: boolean;//Served/Not served
    status_new:boolena// New or not new
}
```</pre>|    This module is necessary beacause it will be the main user of the app, we need a way to identication, that provide us the main information about the user and a way to login into the system. |
| Doctor  | interface doctor{<br>id_doctor: int;//easy identification<br> name_doctor: string// identification;<br> email_doctor:string//information<br> password_doctor: string//Login info; <br> gender_doctor: string;//Some appointment would be necesary to know the gender <br>status_doctor: boolean;//Connected/disconnected <br>list_patient: list;//control of patients<br> number_patients: int;//control of patients<br> hours_available: int//control of appointment <br> schedule_doctor:list//To fix an appointment   <br> status_new:boolean// New or not new   | This module is important beacause the doctor will be able to give tha available hours and days, they will be able to see the active patients and a to put their status to answer a possible quickly contact  |
| Admin | interface admin{<br>id_admin: int;//easy identification <br> email_admin:string//information<br> password_admin: string//Login info;<br> list_new_patient:list;//To update patient list for doctors <br>list_status_patient: list;//to update list for doctors<br>list_new_doctor: list//To accept a new doctor  <br>list_status_doctor: list//To know doctors status <br> list_contact:list//To request information |  This module is necessary for the control of the updated list of patients and doctor, the admin will be able to see the status of both and match the doctors and patients    |
| Auth   | <br> Role based <br>Account creation <br> Account authentication<br> JWT-based  |   This module is necessary for upload new users of the appa and provide authentyfication in the platform   |
| Contact  |  interface contact{<br> name_contact: string// identification;<br> email_contact:string//information<br> status_new:boolena// aswered/not aswered<br>id_message:int;//identification for the direct message   |  Optional: It will helps to exchange direct message between user contacts and doctor/admin    |
| Message  | message_contact:string;<br>answer_doctor:string<br>id_message:int//identification for the direct message     |   This module is necesary to contain the text of the message and match aswer and question for users   |
|  |     |     |

