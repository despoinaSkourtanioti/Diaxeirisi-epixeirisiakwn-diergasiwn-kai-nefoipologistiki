# Διαχείριση Επιχειρησιακών Διεργασιών και Νεφοϋπολογιστική

# Τεχνολογίες:

Python, Microframework Flask, Docker, Kubernetes, MongoDB, HTML

# Περιγραφή Αρχείων:

### 1. docker-compose.yml
Σύνδεση του container με την βάση δεδομένων.

### 2. Dockerfile
Δημιουργία image.

### 3. kubernetes_setup.yml
Περιέχει τα Kubernetes manifests για την ενορχήστρωση των containers στο Kubernetes cluster.

### 4. initialize_db.py
Προσθήκη του admin στο db αν δεν υπάρχει ήδη.

### 5. run.py
Εφαρμογή που περιλαμβάνει τα routes.

### 6. requirements.txt
Τα requirements για να τρέξει το run.py.

### 7. app file
Templates (HTML).

# Τρόπος Εκτέλεσης:

1. git clone
2. CD hospital_management
3. ```kubectl apply -f kubernetes_setup.yaml```
4. ```kubectl get services```
5. Σε ένα browser: http://localhost:<port του flask-service>
###### *π.χ. αν port(s) ```5000:31251/TCP``` τότε http://localhost:31251*

# Τρόπος Χρήσης:

Υπάρχουν 4 collection:
1. users (RBAC)
2. doctors
3. patients
4. appointments

##### Admin credentials:
Username: admin
password: @dm1n

Λειτουργικότητες User:
1. login
2. logout

Λειτουργικότητες Admin:
1. δημιουργία doctor
2. αλλαγή κωδικού doctor
3. διαγραφή doctor
4. διαγραφή patient

Λειτουργικότητες Doctor:
1. αλλαγή κωδικού
2. αλλαγή κόστους
3. προβολή ραντεβού

Λειτουργικότητες Patient:
1. εγγραφη
2. αναζήτηση ραντεβού
3. κράτηση ραντεβού
4. προβολή ραντεβού
5. ακύρωση ραντεβού

# Screenshots:

### Home:
![Screenshot (376)](https://github.com/despoinaSkourtanioti/YpoxreotikiErgasia24_E20148_Skourtanioti_Despoina/assets/137726116/a75eeb01-0426-493a-8802-c8ae520c9f94)
### Admin Dashboard:
![Screenshot (377)](https://github.com/despoinaSkourtanioti/YpoxreotikiErgasia24_E20148_Skourtanioti_Despoina/assets/137726116/66980d60-d4b0-4605-9a52-aee4add86361)
### Δημιουργία doctor:
![Screenshot (378)](https://github.com/despoinaSkourtanioti/YpoxreotikiErgasia24_E20148_Skourtanioti_Despoina/assets/137726116/a00668fa-22e5-4350-bd32-a4640d4ddaeb)
### Doctor Dashboard:
![Screenshot (379)](https://github.com/despoinaSkourtanioti/YpoxreotikiErgasia24_E20148_Skourtanioti_Despoina/assets/137726116/6c833e9f-1044-4734-98e1-2db2cd62686c)
### Αλλαγή κόστους:
![Screenshot (380)](https://github.com/despoinaSkourtanioti/YpoxreotikiErgasia24_E20148_Skourtanioti_Despoina/assets/137726116/89e0ee66-365e-4714-b6f0-dd7a9735b7f0)
### Register:
![Screenshot (381)](https://github.com/despoinaSkourtanioti/YpoxreotikiErgasia24_E20148_Skourtanioti_Despoina/assets/137726116/edeeba9d-2bcc-45b7-9a98-1cf97442fff3)
### Patient Dashboard:
![Screenshot (55)](https://github.com/user-attachments/assets/e541fe9f-458b-4ff2-a37f-679b1cb36e3a)
### Αναζήτηση ραντεβού
![Screenshot (383)](https://github.com/despoinaSkourtanioti/YpoxreotikiErgasia24_E20148_Skourtanioti_Despoina/assets/137726116/81244650-55c4-4cad-a4ed-0fb09d3e7a9d)
### Κράτηση ραντεβού
![Screenshot (384)](https://github.com/despoinaSkourtanioti/YpoxreotikiErgasia24_E20148_Skourtanioti_Despoina/assets/137726116/d28e4365-67b2-4f2d-8dd3-c1286812889f)
### Προβολή λεπτομερειών ραντεβού:
![Screenshot (386)](https://github.com/despoinaSkourtanioti/YpoxreotikiErgasia24_E20148_Skourtanioti_Despoina/assets/137726116/38754e2d-135b-4e75-8277-e0b22b51f751)
### Προβολή ραντεβού signed in ως doctor:
![Screenshot (387)](https://github.com/despoinaSkourtanioti/YpoxreotikiErgasia24_E20148_Skourtanioti_Despoina/assets/137726116/c4313310-8a80-480c-afdd-bf898cc89e7c)
### Η "προβολή ραντεβού" (signed in σαν patient) μετά τη διαγραφή του doctor από τον admin:
![Screenshot (388)](https://github.com/despoinaSkourtanioti/YpoxreotikiErgasia24_E20148_Skourtanioti_Despoina/assets/137726116/5cb9ed23-b757-46f8-95fa-1da13c8a7947)
