Basic XML Layouts
1. Containers
Linear Layout -> modeling tool paling umum , mirip dengan Java-Swing-Box-Layout
Generally, UI design adalah hasil kombinasi dari simpler nested boxes menggunakan horizontal dan vertikal orientation
Terdapat beberapa hal yang sering dipakai pada Android containers
LinearLayout, relativeLayout,TableLayout, ScrollView, dan other(ListView, GridView, WebView, MapView, dll)

Frame Layout : layout manager dari android paling simpel
Terdapat hirarki viewer
1. DecorVIew
2. LinearLayout
3. FrameLayout
4. TextView (dibawah lagi ada komponen" seperti checkbox, radiobutton, button)

LinearLayout :
1. Orientation(indikator sebagai representasi baris/kolom)
bisa dengan menambahkan properti andorid:orientation pada elemen linearlayout
Orientasi bisa di modifikasi dengan fungsi setOrientational()
2. Fill Model
semua widget didalam linearlayout harus dengan atribut android:layout_width dan android:layout_height
3. Gravity
berguna untuk mengontrol posisi button pada layar
4. Padding
banyaknya space antara batasan widget sel dan isi widget content
komponen properti :  android:padding atau dengan setpadding()
5. Marging
untuk mengatur space antara widget dan padding

Relative Layout
adalah tempat widget berdasarkan dengan relationship antara widget lain dalam container
beberapa properti relative layout :
android:layout_allignParentTop
android:layout_allignParentBottom
android:layout_allignParentLeft
android:layout_allignParentRight
dll.

Table Layout
untuk mengatur tata letak widget dalam sebuah grid (baris dan kolom)
dengan komponen properti android:layout_span

Scroll View
menggunakan scroll view saat kita memiliki banyak data yang harus ditampilkan pada single screen

MVVM Java Intro (video youtube)
1.	Data Binding
untuk mengikat data langsung ke file xml
2.	ViewModel
untuk menyimpan data yang lifecycle aware
3. Live Data
untuk autoupdate, aplikasi jadi responsive
4. Navigation Comp
untuk navigasi antar screen
5. RecyclerView
widget wajib hampir selalu dipakai
6. Room Presistence 
untuk solusi database lokal di app
7. Retrofit Library untuk REST API
