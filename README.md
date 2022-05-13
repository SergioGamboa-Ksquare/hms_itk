# Health Management System
# Final Project
## Sergio Gamboa

<table>
<tr>
    <td> Module </td> <td> Code </td><td> Description</td>
</tr>
<tr>
<td> Patient </td>
<td>


```ts

 interface patient{
    id_patient: int;//easy identification
    name_patient: string;// identification
    email_patient:string;//information
    password_patient: string;//Login info
    age_patient:  int//patient info
    gender_patient: string;//Some appointment would be necesary to know the gender
    status_patient: boolean;//Served/Not served
    status_new:boolean;// New or not new
}
```


</td>
    <td> This module is necessary beacause it will be the main user of the app, we need a way to identication, that provide us the main information about the user and a way to login into the system. </td>
</tr>

    
<tr>
<td> Doctor </td>
<td>


```ts

 interface doctor{
    id_doctor: int;//easy identification 
    name_doctor: string;// identification
    email_doctor:string;//information
    password_doctor: string;//Login info
    gender_doctor: string;//Some appointment would be necesary to know the gender
    status_doctor: boolean;//Connected/disconnected 
    list_patient: list;//control of patients
    number_patients: int;//control of patients 
    hours_available: int;//control of appointment 
    schedule_doctor:list;//To fix an appointment
    status_new:boolean;// New or not new  
}
```


</td>
    <td> This module is important beacause the doctor will be able to give tha available hours and days, they will be able to see the active patients and a to put their status to answer a possible quickly contact. </td>
</tr>

    
<tr>
<td> Auth </td>
<td>


```ts

interface admin{
    id_admin: int;//easy identification 
    email_admin:string;//information
    password_admin: string;//Login info
    list_new_patient:list;//To update patient list for doctors
    list_status_patient: list;//to update list for doctors
    list_new_doctor: list;//To accept a new doctor
    list_status_doctor: list;//To know doctors status
    list_contact:list;//To request information
}
```


</td>
    <td> This module is necessary for the control of the updated list of patients and doctor, the admin will be able to see the status of both and match the doctors and patients. </td>
</tr>
    
<tr>
<td> Admin </td>
<td>


<br> Role based <br>Account creation <br> Account authentication<br> JWT-based 


</td>
    <td> This module is necessary for upload new users of the appa and provide authentyfication in the platform </td>
</tr>
    
 <tr>
<td> Contact </td>
<td>

    
```ts    
interface contact{
  name_contact: string;// identification
  email_contact:string;//information
  status_new:boolean;// aswered/not aswered
  id_message:int;//identification for the direct message
}
```


</td>
    <td> Optional: It will helps to exchange direct message between user contacts and doctor/admin </td>
</tr>
<td> Message </td>
<td>

    
```ts    
interface message{
    message_contact:string;//message waiting to receive an answer
    answer_doctor:string;//message to send an answer
    id_message:int;//identification for the direct message
}
```


</td>
    <td> This module is necesary to contain the text of the message and match aswer and question for users </td>
</tr>
</table>


