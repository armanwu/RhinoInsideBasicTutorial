# Tutorial Dasar Rhino.Inside.Revit
Ini adalah salah satu materi dari Modul Layanan Komputasi mata kuliah AR3290 Arsitektur ITB pada tanggal 1 April 2024. Fokus dari materi ini adalah penggunaan Rhino.Inside.Revit sebagai penghubung antara Revit sebagai BIM Authoring Tools dengan Rhino+Grasshopper sebagai Visual Programming untuk Parametric Design. Di akhir materi akan diperkenalkan sekilas mengenai penggunaan Veras sebagai AI Render.

## Software yang Diperlukan

Materi di tutorial ini menggunakan Revit 2023.1, Rhino 7 SR36, Grasshopper 1.0.0007, Rhino.Inside.Revit 1.0, dan Veras 1.6.4.0. Sebelum memulai materi ini, sebaiknya melakukan instalasi software-software tersebut:

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

## 2 Membuat Massa Bangunan di Revit

### 2.1 Menggunakan In-Place Mass
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

## 3 Membuat Lantai, Dinding, dan Atap

### 3.1 Membuat Floor dengan Mass Floor
![Floor_Wall_Roof-1](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(1).png)
1. Pilih geometri massa.
2. Pilih Mass Floors.
3. Pilih lantai yang ingin dibuat.
4. Klik Ok.

![Floor_Wall_Roof-2](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(9).png)
1. Pilih menu Massing & Site.
2. Pilih Floor.

![Floor_Wall_Roof-3](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(10).png)
1. Pilih jenis lantai yang dibutuhkan di Properties.
2. Klik Mass Floors yang inging dijadikan Floor.
3. Klik Create Floor.

### 3.2 Membuat Wall
![Floor_Wall_Roof-4](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(11).png)
1. Pilih menu Massing & Site.
2. Pilih Wall.

![Floor_Wall_Roof-5](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(12).png)
1. Pilih jenis dinding yang dibutuhkan di Properties.
2. Pilih posisi dinding yang dibutuhkan terhadap bidang massa di Location Line.
3. Pilih bidang massa yang ingin dijadikan dinding.

### 3.3 Membuat Roof
![Floor_Wall_Roof-6](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(13).png)
1. Pastikan bidang massa yang akan dijadikan atap terlihat di 3D view.
2. Pilih menu Massing & Site.
3. Pilih Roof.

![Floor_Wall_Roof-7](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(14).png)
1. Pilih jenis atap yang dibutuhkan di Properties.
2. Pilih posisi atap terhadap bidang massa di Picked Faces Location.
3. Pilih bidang massa yang ingin dijadikan atap.

### 3.4 Merapikan Roof
![Floor_Wall_Roof-8](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(15).png)
1. Klik atap kemudian klik Align atau gunakan shortcut AL.
2. Klik bidang dinding sebagai acuan, kemudian klik bidang atap yang ingin disesuaikan.

### 3.5 Menyembunyikan Grid dan Level di 3D View
![Floor_Wall_Roof-9](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(16).png)
1. Klik Visibility/Graphic Overrides atau gunakan shortcut VG.
2. Pilh tab Annotation Categories.
3. Matikan centang di Show annotation categories in this view.
4. Klik Ok.

### 3.6 Menyembunyikan Mass dan Mass Floor
![Floor_Wall_Roof-10](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(17).png)
1. Pilih semua objek di tampilan 3D view.
2. Pilih Filter.
3. Pilih Mass dan Mass Floor saja.
4. Klik Ok.

![Floor_Wall_Roof-11](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/03-Floor_Wall_Roof%20(18).png)
1. Klik kanan kemudian pilih Hide in View.
2. Pilih Elements.

## 4 Menghubungkan Model Revit ke Rhino+GH

### 4.1 Menjalankan Rhino.Inside.Revit
![Revit_to_Grasshopper-1](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/04-Revit_to_Grasshopper%20(1).png)
1. Pilih Menu Rhino.Inside kemudian pilih Start.
2. Pilih Grasshopper untuk menampilkan jendela Grasshopper.
3. Pilih Open Viewport untuk menampilkan jendela Rhino Viewport.

### 4.2 Menggunakan Graphical Element
![Revit_to_Grasshopper-2](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/04-Revit_to_Grasshopper%20(2).png)
1. Di jendela Grasshopper, pilih tab Params.
2. Pilih Revit.
3. Pilih Graphical Element, kemudian tempatkan di canvas Grasshopper.

![Revit_to_Grasshopper-3](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/04-Revit_to_Grasshopper%20(3).png)
1. Klik kanan di Graphical Element, kemudian pilih Set Multiple Graphical Elements.

![Revit_to_Grasshopper-4](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/04-Revit_to_Grasshopper%20(4).png)
1. Pilih semua objek yang ada di tampilan 3D view Revit.
2. Klik Finish.

### 4.3 Membuat Garis Acuan untuk Secondary Skin
![Revit_to_Grasshopper-5](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/04-Revit_to_Grasshopper%20(5).png)
1. Kembali ke Revit, kemudian pilih menu Architecture.
2. Pilih Model Line.
3. Buat garis acuan untuk posisi secondary skin.

### 4.4 Menyesuaikan Level untuk Secondary Skin
![Revit_to_Grasshopper-6](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/04-Revit_to_Grasshopper%20(6).png)
1. Buat Graphical Element baru kemudian hubungkan dengan garis acuan di Revit.
2. Ubah Graphical Element tersebut menjadi Curve.
3. Buat Move to Point kemudian hubungkan Curve ke Geometry.
4. Buat dua Add Level untuk Level 0 dan Level 1, kemudian hubungkan Level 0 ke Point A dan Level 1 ke Point B.

## 5 Membuat Secondary Skin di Grasshopper
![Facade-1](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/05-Facade%20(2).png)
1. Buat Extrude kemudian hubungkan garis hasil Move to Point sebelumnya dengan Base.
2. Buatlah Unit Vector Z kemudian berikan nilai dengan Number Slider, dan dihubungkan dengan Direction di Extrude.

![Facade-2](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/05-Facade%20(3).png)
1. Ikuti gambar.
2. Gunakan Deconstruct Brep untuk memecah hasil Extrude.
3. Hubungkan Faces dengan Surface dan Edges dengan Line.
4. Hubungkan Surface dengan Divide Surface kemudian hubungkan Points dengan Vertices di Polyline. Sesuaikan U Count dengan Number Slider.
5. Hubungkan Polyline dan Line dengan Curve di Pipe.
6. Sesuaikan Number Slider untuk Radius masing-masing Pipe.

## 6 Menghubungkan Geometri Rhino+GH ke Revit

### 6.1 Menggunakan Add DirectShape (Geometry)
![Grasshopper_to_Revit-1](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/06-Grasshopper_to_Revit%20(1).png)
1. Buat Add DirectShapre (Geometry).
2. Hubungkan semua Pipe ke Geometry, agar semau geometri tersebut tampil di Revit.

### 6.2 Menentukan Kategori
![Grasshopper_to_Revit-2](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/06-Grasshopper_to_Revit%20(2).png)
1. Buat Built-In Categories, pilih Curtain Systems, kemudian hubungkan ke Category di DirectShape.
2. Cek kategori geometri yang sudah dikirim ke Revit, apakah sudah sesuai atau belum. 

### 6.3 Menentukan Material
![Grasshopper_to_Revit-3](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/06-Grasshopper_to_Revit%20(3).png)
1. Buat Query Materials, dan berikan input nama material di Name. Nama material sesuai dengan daftar material di Revit.
2. Buat Material Graphics dan hubungkan ouput Materials dari Query Materials ke input Material di Material Graphics.

![Grasshopper_to_Revit-4](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/06-Grasshopper_to_Revit%20(4).png)
1. Hubungkan output Material dari Material Graphics ke Material di DirectShape.
2. Cek material geometri yang sudah dikirim ke Revit, apakah sudah sesuai atau belum.

## 7 Mengatur View dan Tampilan

### 7.1 Mengatur Camera di 3D View
![View-1](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/07-View%20(1).png)
1. Kembali ke Revit, kemudian pilih denah lantai dasar. Dalam materi ini adalah Level 0.
2. Pilih menu View.
3. Pilih 3D View.
4. Pilih Camera.

![View-2](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/07-View%20(2).png)
1. Tentukan posisi kamera.
2. Tentukan posisi target atau arah kamera.

### 7.2 Mengatur Tampilan Grafis
![View-3](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/07-View%20(3).png)
1. Sesuaikan ukuran dan batas view dari kamera.
2. Pilih Visual Style.
3. Pilih Graphic Display Options.

![View-4](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/07-View%20(4).png)
1. Atur tampilan sesuai keinginan atau kebutuhan.
2. Klik Apply untuk melihat hasilnya.
3. Klik Ok bila sudah selesai mengatur.

## 8 Render dengan AI (Materi Tambahan)
Ini hanyalah sekedar pengenalan akan tampilan UI dari aplikasi Veras yang dijalankan di Revit. Materi ini akan diberikan di kesempatan lain.

![Veras](https://github.com/armanwu/RhinoInsideBasicTutorial/blob/main/Images/08-Veras%20(2).png)

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
