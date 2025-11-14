# HospitalManagementSystem

<h1>Functions</h1>

<h1>Admin</h1>
<ul>
  <li>Signup their account. Then Login (No approval Required).</li>
  <li>Can register/view/approve/reject/delete doctor (approve those doctor who applied for job in their hospital).</li>
  <li>Can admit/view/approve/reject/discharge patient (discharge patient when treatment is done).</li>
  <li>Can Generate/Download Invoice pdf (Generate Invoice according to medicine cost, room charge, doctor charge and other charge).</li>
  <li>Can view/book/approve Appointment (approve those appointments which is requested by patient).</li>
</ul>

<h1>Doctor</h1>
<ul>
  <li>Apply for job in hospital. Then Login (Approval required by hospital admin, Then only doctor can login).</li>
  <li>Can only view their patient details (symptoms, name, mobile) assigned to that doctor by admin.</li>
  <li>Can view their discharged (by admin) patient list.</li>
  <li>Can view their Appointments, booked by admin.</li>
  <li>Can delete their Appointment, when doctor attended their appointment.</li>
</ul>

<h1>Patient</h1>
<ul>
  <li>Create account for admit in hospital. Then Login (Approval required by hospital admin, Then only patient can login).</li>
  <li>Can view assigned doctor's details like (specialization, mobile, address).</li>
  <li>Can view their booked appointment status (pending/confirmed by admin).</li>
  <li>Can book appointments (approval required by admin).</li>
  <li>Can view/download Invoice pdf (Only when that patient is discharged by admin).</li>
</ul>

<h1>HOW TO RUN THIS PROJECT</h1>
<ul>
  <li>Install Python(3.7.6) (Dont Forget to Tick Add to Path while installing Python).</li>
  <li>Open Terminal and Execute Following Commands :</li>
</ul>
pip install django==3.0.5<br>
pip install django-widget-tweaks<br>
pip install xhtml2pdf<br><br><br><br>

<ul>
  <li>Download This Project Zip Folder and Extract it</li>
  <li>Move to project folder in Terminal. Then run following Commands :</li>
</ul>

py manage.py makemigrations<br>
py manage.py migrate<br>
py manage.py runserver<br><br><br><br>

<ul>
  <li>Now enter following URL in Your Browser Installed On Your Pc</li>
</ul>

<h1>CHANGES REQUIRED FOR CONTACT US PAGE</h1>

<ul>
  <li>In settins.py file, You have to give your email and password</li>
</ul>

EMAIL_HOST_USER = 'youremail@gmail.com'<br>
EMAIL_HOST_PASSWORD = 'your email password'<br>
EMAIL_RECEIVING_USER = 'youremail@gmail.com'<br><br><br><br>

<ul>
  <li>Login to gmail through host email id in your browser and open following link and turn it ON</li>
</ul>

https://myaccount.google.com/lesssecureapps

<h1>Drawbacks/LoopHoles</h1>

<ul>
  <li>Any one can be Admin. There is no Approval required for admin account. So you can disable admin signup process and use any logic like creating superuser.</li>
  <li>There should be at least one doctor in hospital before admitting patient. So first add doctor.</li>
  <li>On update page of doctor/patient you must have to update password.</li>
</ul>

<h1>Disclaimer</h1>

<ul>
  <li>This project is developed for demo purpose and it's not supposed to be used in real application.</li>
</ul>
