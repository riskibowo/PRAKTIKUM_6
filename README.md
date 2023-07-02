# PRAKTIKUM_6
_NAMA : RISKI PROBO SADEWO_

### 1 PENGOLAHAN DATA KARYAWAN
### Tabel Departement
### Di bawah ini merupakan perintah dan juga hasil yang di minta
```
CREATE TABLE Departemen ( IDDepartemen INT PRIMARY KEY, NamaDepartemen VARCHAR(255) );
```
![image](https://github.com/riskibowo/PRAKTIKUM_6/assets/115862112/75ac0dc5-8931-4817-a58c-adc0ae8b47ef)
### Tabel Karyawan
### Selanjutnya adalah table karyawan dengan menggunakan perintah seperti di bawah ini beserta hasil
```
CREATE TABLE Karyawan ( IDKaryawan INT PRIMARY KEY, NamaKaryawan VARCHAR(255), IDSupervisor INT, IDDepartemen INT, FOREIGN KEY (IDSupervisor) REFERENCES Karyawan(IDKaryawan), FOREIGN KEY (IDDepartemen) REFERENCES Departemen(IDDepartemen) )
```
![image](https://github.com/riskibowo/PRAKTIKUM_6/assets/115862112/5f7f1a2e-8823-45b8-b7de-2672386bcc5c)
### Tabel Proyek
### Kemudian kita akan melanjutkan pada tabel proyek dengan menggunakan perintah sepert di bawah ini beserta hasilnya
```
CREATE TABLE Proyek ( IDProyek INT PRIMARY KEY, NamaProyek VARCHAR(255), TanggalMulai DATE, TanggalSelesai DATE );
```
![image](https://github.com/riskibowo/PRAKTIKUM_6/assets/115862112/caa8e04e-509f-4d67-b554-0785b88db103)
### Tabel Supervisor
### Kemudian kita akan melanjutkan pada tabel supervisor dengan menggunakan perintah sepert di bawah ini beserta hasilnya
```
CREATE TABLE Supervisor ( IDSupervisor INT, IDDepartemen INT, FOREIGN KEY (IDSupervisor) REFERENCES Karyawan(IDKaryawan), FOREIGN KEY (IDDepartemen) REFERENCES Departemen(IDDepartemen) );
```
![image](https://github.com/riskibowo/PRAKTIKUM_6/assets/115862112/745be18a-57e7-4f78-8160-f8f0ce3d4a07)

### Table Partisipasi
### Kemudian kita akan melanjutkan pada tabel partisipasi dengan menggunakan perintah sepert di bawah ini beserta hasilnya
```
CREATE TABLE Partisipasi ( IDKaryawan INT, IDProyek INT, FOREIGN KEY (IDKaryawan) REFERENCES Karyawan(IDKaryawan), FOREIGN KEY (IDProyek) REFERENCES Proyek(IDProyek) );
```
![image](https://github.com/riskibowo/PRAKTIKUM_6/assets/115862112/9d9cdfd9-13d9-461e-9491-89114157ae30)


