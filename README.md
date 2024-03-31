# Tutorial Dasar Rhino.Inside.Revit
Ini adalah salah satu materi dari Modul Layanan Komputasi mata kuliah AR3290 Arsitektur ITB pada tanggal 1 April 2024. Fokus dari materi ini adalah penggunaan Rhino.Inside.Revit sebagai penghubung antara Revit sebagai BIM Authoring Tools dengan Rhino+Grasshopper sebagai Visual Programming untuk Parametric Design. Di akhir materi akan diperkenalkan sekilas mengenai penggunaan Veras sebagai AI Render.

## Software yang Diperlukan

Sebelum memulai materi ini, sebaiknya melakukan instalasi software-software berikut:

- [Autodesk Revit](https://www.autodesk.com/education/edu-software/)

- [Rhinoceros](https://www.rhino3d.com/for/education/)

- [Rhino.Inside.Revit](https://www.rhino3d.com/inside/revit/)

- [Veras](https://www.evolvelab.io/veras) (optional)

## 1 Membuat Grid dan Level di Revit

### 1.1 Membuat File RVT Baru
![Grid_Level-1](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/01-Grid_Level%20(1).png)
1. Buka Revit dan pilih New Models.
2. Pilih Architectural Template atau template apapun yang sesuai dengan kebutuhan.
3. Klik Ok.

### 1.2 Membuat Grid di Denah
![Grid_Level-2](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/01-Grid_Level%20(2).png)
1. Pilih denah lantai dasar. Contoh di sini adalah Level 0.
2. Pilih menu Architecture.
3. Pilih Grid.
4. Buat Grid di denah lantai dasar. Contoh di sini menggunakan jarak per 8 meter.

### 1.3 Membuat dan Merapikan Level di Tampak
![Grid_Level-3](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/01-Grid_Level%20(3).png)
1. Buka tampak atau elevations.
2. Pilih menu Architecture.
3. Pilih Level.
4. Buat Level sesuai kebutuhan dan rapikan semua view tampak. Contoh di sini membuat sampai Level 3.

### 1.4 Menampilkan Grid dan Level di 3D View
![Grid_Level-4](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/01-Grid_Level%20(4).png)
1. Buka 3D view.
2. Atur viewnya dengan Navigation Tools.
3. Buka Show Grids, kemudian aktifkan agar grid tampil di 3D view.
4. Pastikan grid dan level tampil di 3D view.

## 2 Membuat Massa Bangunan dengan In-Place Mass

### 2.1 Memulai In-Place Mass
![Mass-1](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/02-Mass%20(1).png)
1. Pilih menu Massing & Site.
2. Pilih In-Place Mass.
3. Masukkan nama untuk Mass-nya atau biarkan saja sesuai default.
4. Klik Ok.

### 2.2 Membuat Form
![Mass-2](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/02-Mass%20(2).png)
1. Pilih Model.
2. Pilih Rectangle.
3. Buat geometri rectangle berdasarkan acuan grid.
4. Pilih Create Form.

### 2.3 Mengatur Form
![Mass-3](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/02-Mass%20(3).png)
1. Pilih Align.
2. Klik garis Level paling atas.
3. Klik permukaan massa paling bagian atas.

### 2.4 Membagi segmen dengan Add Edge
![Mass-4](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/02-Mass%20(4).png)
1. Klik salah satu bagian dari geometri massa.
2. Pilih Add Edge
3. Buat garis di bidang samping atau dinding geometri massa.
4. Klik Finish Mass.

## 3 Membuat Lantai, Dinding, dan Atap dengan Massing

### 3.1 Membuat Floor dengan Mass Floor
![Floor_Wall_Roof-1](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(1).png)

![Floor_Wall_Roof-2](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(9).png)

![Floor_Wall_Roof-3](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(10).png)

### 3.2 Membuat Wall
![Floor_Wall_Roof-4](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(11).png)

![Floor_Wall_Roof-5](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(12).png)

### 3.3 Membuat Roof
![Floor_Wall_Roof-6](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(13).png)

![Floor_Wall_Roof-7](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(14).png)

### 3.4 Merapikan Roof
![Floor_Wall_Roof-8](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(15).png)

### 3.5 Menyembunyikan Grid dan Level di 3D View
![Floor_Wall_Roof-9](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(16).png)

### 3.6 Menyembunyikan Mass dan Mass Floor
![Floor_Wall_Roof-10](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(17).png)

![Floor_Wall_Roof-11](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(18).png)

## 4 Menghubungkan Model Revit ke Rhino+GH

### 4.1 Menjalankan Rhino.Inside.Revit
![Revit_to_Grasshopper-1](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/04-Revit_to_Grasshopper%20(1).png)

### 4.2 Menggunakan Graphical Element
![Revit_to_Grasshopper-2](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/04-Revit_to_Grasshopper%20(2).png)

![Revit_to_Grasshopper-3](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/04-Revit_to_Grasshopper%20(3).png)

![Revit_to_Grasshopper-4](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/04-Revit_to_Grasshopper%20(4).png)

### 4.3 Membuat Garis Acuan untuk Secondary Skin Di Revit
![Revit_to_Grasshopper-5](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/04-Revit_to_Grasshopper%20(5).png)

### 4.4 Menyesuaikan Posisi Secondary Skin terhadap Level
![Revit_to_Grasshopper-6](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/04-Revit_to_Grasshopper%20(6).png)

## 5 Membuat Secondary Skin di Grasshopper

![Facade-1](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/05-Facade%20(2).png)

![Facade-2](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/05-Facade%20(3).png)

## 6 Menghubungkan Geometri Rhino+GH ke Revit

![Grasshopper_to_Revit-1](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/06-Grasshopper_to_Revit%20(1).png)
![Grasshopper_to_Revit-2](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/06-Grasshopper_to_Revit%20(2).png)
![Grasshopper_to_Revit-3](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/06-Grasshopper_to_Revit%20(3).png)
![Grasshopper_to_Revit-4](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/06-Grasshopper_to_Revit%20(4).png)

## Tautan Video Youtube
[Klik di sini](https://youtu.be/HsxuzNzMt2A) untuk melihat video penjelasan materi ini di Youtube.

## File Contoh

- [File contoh RVT dan GH](https://github.com/armanwu/RhinoInsideBasicTutorial/tree/main/Sample_Files).

- [File contoh hasil AI Render](https://github.com/armanwu/RhinoInsideBasicTutorial/tree/main/Sample_Render).

## Referensi

- [BIM + Computational Design + AI menggunakan Revit, Rhino.Inside, Grasshopper, dan Veras](https://youtu.be/HsxuzNzMt2A)

- [Rhino.Inside.Revit Guides](https://www.rhino3d.com/inside/revit/1.0/guides/)

- [Konsep Massa Bangunan di Revit menggunakan In-Place Mass bagian 1](https://youtu.be/zNI8fCXr3Ow?si=yAzj4EV8YX9lS-by)

- [Konsep Massa Bangunan di Revit menggunakan In-Place Mass bagian 2](https://youtu.be/1fWu17E0JEU?si=zGPVEaBHnNsmQAK7)

- [Massing Studies](https://help.autodesk.com/view/RVTLT/2024/ENU/?guid=GUID-B8858693-F46D-4211-8CCC-B5E88681C466)

- [Create an In-Place Mass](https://help.autodesk.com/view/RVTLT/2024/ENU/?guid=GUID-A180B32D-E7B8-474F-AB31-B15EDB874F6E)



