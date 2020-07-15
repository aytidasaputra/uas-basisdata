## PRAKTIKUM BASISDATA INFORMATIKA

```sql
1. CREATE DATABASE aditya_saputra528;
```

```sql
2. CREATE TABLE `aditya_saputra528`.`buku` (
  `kd_buku` INT NOT NULL,
  `judul` VARCHAR(45) NULL,
  `jenis_buku` VARCHAR(45) NULL,
  `pengarang` VARCHAR(45) NOT NULL,
  `jml_buku` INT NOT NULL,
  PRIMARY KEY (`kd_buku`));
CREATE TABLE `aditya_saputra528`.`buku` (
);


INSERT INTO `aditya_saputra528`.`buku` (`kd_buku`, `judul`, `jenis_buku`, `pengarang`, `jml_buku`) VALUES ('BK001', 'Laskar Pelangi', 'Novel', 'Andrea Hirata', '12');
INSERT INTO `aditya_saputra528`.`buku` (`kd_buku`, `judul`, `jenis_buku`, `pengarang`, `jml_buku`) VALUES ('BK002', 'Cantik Itu Luka', 'Novel', 'Eka Kurniawan', '6');
INSERT INTO `aditya_saputra528`.`buku` (`kd_buku`, `judul`, `jenis_buku`, `pengarang`, `jml_buku`) VALUES ('BK003', 'Rentang Kisah', 'Novel', 'Gita Savitri Devi', '8');
INSERT INTO `aditya_saputra528`.`buku` (`kd_buku`, `judul`, `jenis_buku`, `pengarang`, `jml_buku`) VALUES ('BK004', 'Aku', 'Sastra', 'Sjuman Djaya', '18');
INSERT INTO `aditya_saputra528`.`buku` (`kd_buku`, `judul`, `jenis_buku`, `pengarang`, `jml_buku`) VALUES ('BK005', 'Kereta Tidur', 'Sastra', 'Avianty Armand', '20');
INSERT INTO `aditya_saputra528`.`buku` (`kd_buku`, `judul`, `jenis_buku`, `pengarang`, `jml_buku`) VALUES ('BK006', 'Laluba', 'Sastra', 'Nukila Amal', '15');
INSERT INTO `aditya_saputra528`.`buku` (`kd_buku`, `judul`, `jenis_buku`, `pengarang`, `jml_buku`) VALUES ('BK007', 'Panggil Aku Kartini Saja', 'Biografi', 'Pramoedya Ananta Toer', '10');
INSERT INTO `aditya_saputra528`.`buku` (`kd_buku`, `judul`, `jenis_buku`, `pengarang`, `jml_buku`) VALUES ('BK008', 'Chairil', 'Biografi', 'Hasan Aspharani', '20');
INSERT INTO `aditya_saputra528`.`buku` (`kd_buku`, `judul`, `jenis_buku`, `pengarang`, `jml_buku`) VALUES ('BK009', 'Ensiklopedia Antariksa', 'Ensiklopedia', 'James Trefil', '12');
INSERT INTO `aditya_saputra528`.`buku` (`kd_buku`, `judul`, `jenis_buku`, `pengarang`, `jml_buku`) VALUES ('BK010', 'Ensiklopedia Sains', 'Ensiklopedia', 'Damaring Tyas', '6');


CREATE TABLE `aditya_saputra528`.`pinjam` (
  `kd_pinjam` INT NOT NULL AUTO_INCREMENT,
  `no_anggota` VARCHAR(45) NOT NULL,
  `kd_buku` INT NOT NULL,
  `tgl_pinjam` DATE NOT NULL,
  `tgl_kembali` DATE NOT NULL,
  PRIMARY KEY (`kd_pinjam`));

INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('1', 'AG004', '001', '22/05/2017', '29/05/2017');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('2', 'AG004', '003', '22/05/2017', '29/05/2017');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('3', 'AG001', '004', '23/05/2017', '30/05/2017');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('4', 'AG001', '003', '23/05/2017', '30/05/2017');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('5', 'AG003', '001', '23/05/2017', '30/05/2017');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('6', 'AG002', '002', '24/05/2017', '01/06/2017');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('7', 'AG002', '010', '24/05/2017', '01/06/2017');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('8', 'AG005', '006', '24/05/2017', '01/06/2017');

INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('1', 'AG004', '001', '2017-05-22', '2017-05-29');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('2', 'AG004', '003', '2017-05-22', '2017-05-29');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('3', 'AG001', '004', '2017-05-23', '2017-05-30');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('4', 'AG001', '003', '2017-05-23', '2017-05-30');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('5', 'AG003', '001', '2017-05-23', '2017-05-30');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('6', 'AG002', '002', '2017-05-24', '2017-06-01');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('7', 'AG002', '010', '2017-05-24', '2017-06-01');
INSERT INTO `aditya_saputra528`.`pinjam` (`kd_pinjam`, `no_anggota`, `kd_buku`, `tgl_pinjam`, `tgl_kembali`) VALUES ('8', 'AG005', '006', '2017-05-24', '2017-06-01');


CREATE TABLE `aditya_saputra528`.`anggota` (
  `no_anggota` INT NOT NULL,
  `indentitas` VARCHAR(45) NOT NULL,
  `nama_anggota` VARCHAR(45) NOT NULL,
  `alamat` VARCHAR(80) NOT NULL,
  PRIMARY KEY (`no_anggota`));

INSERT INTO `aditya_saputra528`.`anggota` (`no_anggota`, `indentitas`, `nama_anggota`, `alamat`) VALUES ('1', 'KTM', 'Ibnu Saladdin', 'Jalan Anyelir 22, Jakarta');
INSERT INTO `aditya_saputra528`.`anggota` (`no_anggota`, `indentitas`, `nama_anggota`, `alamat`) VALUES ('2', 'KTP', 'Kirani Deviana', 'Jalan Melati 18, Depok');
INSERT INTO `aditya_saputra528`.`anggota` (`no_anggota`, `indentitas`, `nama_anggota`, `alamat`) VALUES ('3', 'KTM', 'Afifa Adena', 'Jalan Gabus 23, Bogor');
INSERT INTO `aditya_saputra528`.`anggota` (`no_anggota`, `indentitas`, `nama_anggota`, `alamat`) VALUES ('4', 'SIM', 'Luqyaana', 'Jalan Cangkalang 17, Bogor');
INSERT INTO `aditya_saputra528`.`anggota` (`no_anggota`, `indentitas`, `nama_anggota`, `alamat`) VALUES ('5', 'KTM', 'Reno Athallah', 'Jalan Ruansa 34, Bekasi');
```

```sql
3. SELECT buku.kd_buku
    , buku.judul
    , pinjam.tgl_pinjam
    , pinjam.tgl_kembali
FROM buku
INNER JOIN pinjam 
    on buku.kd_buku = pinjam.kd_pinjam
WHERE pinjam.tgl_pinjam between '2017-05-23' and '2017-05-24';
```

```sql
4. SELECT anggota.nama_anggota
    , anggota.alamat
    , pinjam.tgl_pinjam
    , pinjam.tgl_kembali
FROM buku
INNER JOIN pinjam 
    on buku.kd_buku = pinjam.kd_pinjam
INNER JOIN anggota 
    on buku.kd_buku = anggota.no_anggota;
```


```sql
5. SELECT buku.judul
    , anggota.jenis_buku
FROM buku
INNER JOIN anggota 
    on buku.kd_buku = anggota.no_anggota
WHERE anggota.nama_anggota LIKE '%Luqyaana%';
```

```sql
6. SELECT anggota.nama_anggota
    , buku.judul
    , pinjam.tgl_pinjam
FROM buku
INNER JOIN pinjam 
    on buku.kd_buku = pinjam.kd_pinjam
INNER JOIN anggota 
    on buku.kd_buku = anggota.no_anggota
WHERE anggota.alamat LIKE '%Bogor%';
```

```sql
7. SELECT buku.judul
    , pinjam.kd_pinjam
FROM buku
INNER JOIN pinjam 
    on buku.kd_buku = pinjam.kd_pinjam
INNER JOIN anggota 
    on buku.kd_buku = anggota.no_anggota
WHERE anggota.nama_anggota LIKE '%R%';
```

```sql
8. SELECT anggota.nama_anggota
    , buku.jenis_buku
    , pinjam.tgl_pinjam
    , pinjam.tgl_kembali
FROM buku
INNER JOIN pinjam 
    on buku.kd_buku = pinjam.kd_pinjam
INNER JOIN anggota 
    on buku.kd_buku = anggota.no_anggota
WHERE anggota.nama_anggota LIKE '%KTM%' OR LIKE '%KTP%'
AND pinjam.tgl_pinjam between '2017-05-23' and '2017-05-24';
```

```sql
9. SELECT anggota.nama_anggota
    , pinjam.kd_pinjam
    , buku.jml_buku
FROM buku
INNER JOIN pinjam 
    on buku.kd_buku = pinjam.kd_pinjam
INNER JOIN anggota 
    on buku.kd_buku = anggota.no_anggota
WHERE buku.jml_buku = 2;
```

```sql
10. SELECT anggota.no_anggota
    , anggota.nama_anggota
    , anggota.alamat
    , pinjam.tgl_pinjam
    , pinjam.tgl_kembali
FROM buku
INNER JOIN pinjam 
    on buku.kd_buku = pinjam.kd_pinjam
INNER JOIN anggota 
    on buku.kd_buku = anggota.
WHERE pinjam.tgl_pinjam between '2017-05-29' and '2017-05-30';
```

