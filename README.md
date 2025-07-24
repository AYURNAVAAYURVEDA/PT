<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Patient Medical Record Book</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="medical-record-book">
        <header>
            <h1>Patient Medical Record</h1>
            <p>Confidential Patient Information</p>
        </header>

        <form id="medicalRecordForm" action="#" method="POST">
            <section class="patient-info">
                <h2>Patient Information</h2>
                <div class="form-group">
                    <label for="patientName">Full Name:</label>
                    <input type="text" id="patientName" name="patientName" required>
                </div>
                <div class="form-group">
                    <label for="dob">Date of Birth:</label>
                    <input type="date" id="dob" name="dob" required>
                </div>
                <div class="form-group">
                    <label for="gender">Gender:</label>
                    <select id="gender" name="gender" required>
                        <option value="">Select Gender</option>
                        <option value="male">Male</option>
                        <option value="female">Female</option>
                        <option value="other">Other</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="contactNo">Contact Number:</label>
                    <input type="tel" id="contactNo" name="contactNo" pattern="[0-9]{10}" placeholder="e.g., 07XXXXXXXX" required>
                </div>
                <div class="form-group">
                    <label for="address">Address:</label>
                    <textarea id="address" name="address" rows="3" required></textarea>
                </div>
                <div class="form-group">
                    <label for="emergencyContact">Emergency Contact Name:</label>
                    <input type="text" id="emergencyContact" name="emergencyContact">
                </div>
                <div class="form-group">
                    <label for="emergencyContactNo">Emergency Contact Number:</label>
                    <input type="tel" id="emergencyContactNo" name="emergencyContactNo" pattern="[0-9]{10}" placeholder="e.g., 07XXXXXXXX">
                </div>
            </section>

            <section class="medical-history">
                <h2>Medical History</h2>
                <div class="form-group">
                    <label for="allergies">Allergies (e.g., Penicillin, Peanuts):</label>
                    <textarea id="allergies" name="allergies" rows="2"></textarea>
                </div>
                <div class="form-group">
                    <label for="chronicDiseases">Chronic Diseases (e.g., Diabetes, Hypertension):</label>
                    <textarea id="chronicDiseases" name="chronicDiseases" rows="2"></textarea>
                </div>
                <div class="form-group">
                    <label for="pastSurgeries">Past Surgeries:</label>
                    <textarea id="pastSurgeries" name="pastSurgeries" rows="2"></textarea>
                </div>
                <div class="form-group">
                    <label for="currentMedications">Current Medications:</label>
                    <textarea id="currentMedications" name="currentMedications" rows="2"></textarea>
                </div>
            </section>

            <section class="current-visit">
                <h2>Current Visit Details</h2>
                <div class="form-group">
                    <label for="visitDate">Visit Date:</label>
                    <input type="date" id="visitDate" name="visitDate" required>
                </div>
                <div class="form-group">
                    <label for="chiefComplaint">Chief Complaint:</label>
                    <textarea id="chiefComplaint" name="chiefComplaint" rows="3" required></textarea>
                </div>
                <div class="form-group">
                    <label for="diagnosis">Diagnosis:</label>
                    <textarea id="diagnosis" name="diagnosis" rows="3"></textarea>
                </div>
                <div class="form-group">
                    <label for="treatmentPlan">Treatment Plan:</label>
                    <textarea id="treatmentPlan" name="treatmentPlan" rows="3"></textarea>
                </div>
                <div class="form-group">
                    <label for="prescribedMedications">Prescribed Medications:</label>
                    <textarea id="prescribedMedications" name="prescribedMedications" rows="3"></textarea>
                </div>
                <div class="form-group">
                    <label for="notes">Doctor's Notes:</label>
                    <textarea id="notes" name="notes" rows="4"></textarea>
                </div>
            </section>

            <button type="submit">Save Record</button>
        </form>
    </div>
</body>
</html>
