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
